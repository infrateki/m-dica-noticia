
============================================================
📅 2026-02-07T16:58
📝 Discussion of an Anthropic article on building a C compiler with AI agent teams
ID: UK0Ru8sQEXpRZoM0zPDo
------------------------------------------------------------

## Discussion of an Anthropic article on building a C compiler with AI agent teams


## Introduction to the Anthropic article on AI-powered C compiler development

  [Unknown]: Voy a leer un artículo de Anthropic.
  [Unknown]: de febrero 6 del 2026 de Engineering at Anthropic, se llama building a C compiler with a team of parallel clodes.
  [Unknown]: Dice, we task Opus 4.6 using agent teams to build a C compiler and then mostly walked away.
  [Unknown]: Here's what it taught us about the future of autonomous software development.
  [Unknown]: Published February 5th, 2026, written by Nicolás Carlini, a research on Anthropic Safeguard team.

## Acknowledgments for contributions to the article

  [Unknown]: Special thanks to Joseph Bassich, Edwin Chen, Bernardo Meurer Costa, Jake Eton, Dan Kelly, Felix Clock,
  [Unknown]: Janet Park, Steve Weiss and many other people across Anthropic for their assistance and contributions.

## Overview of agent teams for autonomous software development

  [Unknown]: I've been experimenting with a new approach to supervising language models that we're calling agent teams.
  [Unknown]: With agent teams, multiple cloud instances work in parallel on a shared code base without active human intervention.
  [Unknown]: This approach dramatically expands the scope of what's achievable with LLM agents.

## The C compiler experiment and its impressive results

  [Unknown]: To stress it, to stress test it, I tasked 16 agents with writing a rust based C compiler from scratch, capable of compiling the Linux kernel.
  [Unknown]: Over nearly 2,000 cloud code sessions and $20,000 in API costs, the agent team produced a 100,000 line compiler that can build Linux 6.9 on X86 arm and risk V.

## Key learnings from designing harnesses for autonomous agent teams

  [Unknown]: The compiler is an interesting artifact on its own, but I focus here on what I learned about designing harnesses for long running autonomous agents teams.
  [Unknown]: How to write tests that keep agents on track without human oversight.
  [Unknown]: How to structure work so multiple agents can make progress in parallel and where this approach hits its ceiling.

## Strategies for enabling long-running autonomous agent progress

  [Unknown]: Enabling long running clodes. Existing agent scaffolds like cloud code require an operator to be online and available to work jointly.
  [Unknown]: If you ask for a solution to a long and complex problem, the model may solve part of it, but eventually it will stop and wait for continued input, a question, a status update or a request for clarification.
  [Unknown]: To elicit sustained autonomous progress, I built a harness that sticks cloud in a simple loop.
  [Unknown]: If you've seen Ralph loop, this should look familiar.
  [Unknown]: When it finishes one task, it immediately picks up the next.
  [Unknown]: Run this in a container, not your actual machine.
  [Unknown]: hashtag exclamation forward-bin forward/bash while true do commit equals dollar sign git rev-parse dash dash short equals 6 head close bracket log file equals agent logs agent dollar sign commit log cloud dash dash dangerously skip permissions back slash dash p dollar sign cat agent prompt MD inside brackets back dash dash dash model cloud Opus XY and bracket dollar sign log file done.
  [Unknown]: In the agent prompt, I told cloud what problem to solve and asked it to approach the problem by breaking it into smaller pieces, smaller pieces.
  [Unknown]: Tracking what it's working on, figuring out what to work on next and to effectively keep going until it's perfect.
  [Unknown]: On this last point, cloud has no choice. The loop runs forever.
  [Unknown]: Although, in one instance, I did see cloud P kill-9 passion accident, thus killing itself and ending the loop.
  [Unknown]: Whoops.

## Benefits of running multiple AI agents in parallel for efficiency

  [Unknown]: Running cloud in parallel. Running multiple instances in parallel can address two weaknesses of a single agent harness.
  [Unknown]: One cloud code session can only do one thing at a time, especially as the scope of a project expands.
  [Unknown]: Debugging multiple issues in parallel is far more efficient.
  [Unknown]: Running multiple cloud agents allows for special

## Technical implementation, agent autonomy, and practical lessons from developing with agent teams

  [Unknown]: zation. While a few agents are tasked to solve the actual problem at hand, other specialized agents can be invoked to, for example, maintain documentation, keep an eye on code quality or solve specialized subtasks. My implementation of parallel cloud is bare bones. A new bare Git repo is created and for each agent, a docker container is spun up with the repo mounted to upstream. Each agent clones to local copy to dash workspace and then it's done. Pushes from its own local container to upstream. To prevent two agents from trying to solve the same problem at the same time, the harness uses a simple synchronization algorithm. Cloud takes a lock on a task by writing a text file to current task forward slash. Example, one agent might lock current tasks parse if statement.text while other logs current tasks code gen function definitions text. If two agents try to claim the same task, Git synchronization forces the second agent to pick a different one. Cloud works on the task, then pulls from upstream, merges changes from other agents, push it pushes its changes and removes the lock. Merge conflicts are frequent, but cloud is smart enough to figure that out. That infinite agent generation loop spawns a new cloud code session in a fresh container and the cycle repeats. This is very early research prototype. I haven't yet implemented any other method for communication between agents, nor do I enforce any process for managing high level goals. I don't use an orchestration agent. Instead, I leave it up to each cloud agent to decide how to act. In most cases, cloud picks up the next most obvious problem. When stuck on a bug, cloud will often maintain a running doc of failed approaches and remaining tasks in the Git repository of the project. You can read through the history and watch it take out locks on various tasks. Lessons from programming with cloud agent teams. The scaffolding runs cloud in a loop, but that loop is only useful if cloud can tell how to make progress. Most of the most of my effort went into designing the environment around cloud. The tests, the environment, the feedback so that it could orient itself without me. These are the approaches I found most useful when orchestrating multiple cloud instances. With extremely high quality tests, cloud will work autonomously to solve whatever problem I give it. So it's important that the task verifier is nearly perfect. Otherwise, cloud will solve the wrong problem. Improving the testing harness requires finding high quality compiler test suites, writing verifiers and build scripts for open source software packages and watching for mistakes cloud was making, then designing new tests as I identified those failure modes. For example, near the end of the project, cloud started to frequently break existing functionality each time it implemented a new feature. To address this, I build a continuous integration pipeline and implemented stricter enforcement that allowed cloud to better test its work so that new commits can so that new commits cannot break existing code. Put yourself in cloud's shoes. I had to constantly remind myself that I was writing this tests harness for cloud and not for myself, which meant rethinking many of my assumptions about how tests should communicate results. For example, each agent is dropped into a fresh container with no context and will spend significant time orienting itself, especially on large projects. Before we even reach the tests to help cloud help itself, I included instructions to maintain extensive readmes and progress files that should be updated frequently with the current status. I also kept in mind the fact that language models have inherent limitations which in
  [Unknown]: case needed to be designed around. This includes context window pollution. The test harness should not print thousands of useless bytes at most. It should print a few lines of output and log all important information to a file so cloud can find it when needed. Log files should be easy to process automatically. If there are errors, cloud should write error and put the reason on the same line, so grep will find it. It helps it helps to precompute aggregate summary statistics, so cloud doesn't have to recompute them. Timeliness. Cloud can't tell time and left alone will happily spend hours running tests instead of making progress. The harness print incremental progress infrequently to avoid polluting context and includes a default dash dash fast option that runs a 1% or 10% random sample. That sub sample is deterministic per agent, but random across virtual machines. So cloud still covers all files, but each agent can perfectly identify regressions.
  [Unknown]: Make parallelism easy. When there are many distinct failing tests, parallelization is trivial. Each agent picks a different failing test to work on. After the test suite reached a 99 pass rate, each agent worked on getting a different small open source project. Example, SQL light, Redis, lib JPEG, MQ Quickjs, Lua, etc to compile. But when agents started to compile the Linux kernel, they got stuck. Unlike a test suite with hundreds of independent tests, compiling the Linux kernel is one giant task. Every agent would hit the same bug, fix that bug, and then overwrite each other's changes. Having 16 agents running didn't help because each was stuck solving same task.
  [Unknown]: The fix was to use GCC as an online known good compiler Oracle to compare against. I wrote a new test harness that randomly compiled most of the kernel using GCC and only the remaining files with cloud C compiler. If the kernel worked, then the problem wasn't in cloud subset of the files. If it broke, then it could further refine by recompiling some of these files with GCC. This lets each agent work in parallel, fixing different bugs in different files. With cloud's compiler could eventually compile all files. After this worked, it was still necessary to apply Delta debugging techniques to find pairs of files that failed together, but worked independently.

## Specialized agent roles and project's benchmarking purpose

  [Unknown]: Multiple agent roles. Parallelism also enables specialization. LLM written code frequently reimplements existing functionality. So I tasked one agent with co lessing any duplicate code it found. He put another in charge of improving the performance of the compiler itself. And the third, I made responsible for outputting efficient compiled code. I asked another agent to critique the design of the project from the perspective of a rust developer and make structural changes to the project to improve the overall code quality and another to work on documentation. Stress testing the limits of agent teams. This project was designed as a this project was designed as a capability benchmark. I am interested in stress testing the limits of what LLMs can just barely achieve today in order to help us prepare for what models will reliably achieve in the future. I've been using the C compiler project as a benchmark across the entire cloud four model series. Series. As I did with prior projects. I started by drafting what I wanted. A from scratch optimizing compiler with dependencies GCC comparable able to compile the Linux kernel and designed to support multiple bench backends. And designed to support multiple backends. While I specified some aspects of the design, for example, that it should have a SSA IR to enable multi optimization passes, I did not go into any detail on how to do so. Previous Opus 4 models were barely capable of producing a functional compiler. Opus 4.5 was the first to cross a threshold that allowed it to produce a functional compiler, which could pass large test suites, but it was still incapable of compiling any real large projects. My goal with Opus 4.6 was to again test the limits.

## Comprehensive evaluation of the C compiler's performance, cost, and limitations

  [Unknown]: Evaluation. Over nearly 2,000 cloud code sessions across two weeks, Opus 4.6 consumed 2 billion input tokens and generated 140 million output tokens. A total cost just under $20,000 US. Compared to even the most expensive cloud Max plans, this was an extremely expensive project. But the total is a fraction of what it would cost me to produce this myself. Let alone an entire team. This was a clean room implementation. Cloud did not have internet access at any point during its development. It depends only on the rust standard library. The 100,000 line compiler can build a bootable Linux 6.9 on X86 ARM and risk V. It can also compile QEMU FFMPEG SQL light, Postgres, Redis and has a 99% pass rate on most compiler test suites including the GCC torture test suite. It also passes the developer's ultimate litmus test. It can compile and run Doom. The compiler, however, is not without limitations. This includes it lacks the 16bit X86 compiler that is necessary to boot Linux out of real mode.
  [Unknown]: this, it calls out a GCC.
  [Unknown]: parenthesis, the X86 32 and X86 64 compilers are its own.
  [Unknown]: It does not have its own assembler and linker.
  [Unknown]: These are the very last bits that cloud started automating and are still somewhat buggy.
  [Unknown]: The demo video with a GCC assembler and linker.
  [Unknown]: The compiler successfully builds many projects, but not all.
  [Unknown]: It's not yet a drop in replacement for a real compiler.
  [Unknown]: The generated code is not very efficient.
  [Unknown]: Even with all optimizations enabled, it outputs less efficient code than GCC with all optimizations disabled.
  [Unknown]: The rust code quality is reasonable, but is nowhere near the quality of what an expert rust programmer might produce.
  [Unknown]: The resulting compiler has nearly reached the limits of Opus abilities.
  [Unknown]: I tried hard to fix several of the above limitations, but wasn't fully successful.
  [Unknown]: New features and bug fixes frequently broke existing functionality.
  [Unknown]: As one particular challenging example, Opus was unable to implement a 16 bit X86 code generator needed to boot into 16 bit real mode.
  [Unknown]: While the compiler can output correct 16 bit X86 via the 6667 OP code prefixes, the resulting compiled Opus is over 60 KB, far exceeding 32K code limited forced by Linux.
  [Unknown]: Instead, cloud simply cheats here and calls out a GCC for this phase.
  [Unknown]: This is only the case for X86, for arm or risk V, cloud compiler can compile completely by itself.

## Availability of the compiler, methodology for testing LLMs, and future development plans

  [Unknown]: The source code for compiler is available, download it, read through the code and list on your favorite C projects.
  [Unknown]: I've consistently found the best way to understand what language models can do is to push them to their limits and then study where they start where they start to break down.
  [Unknown]: Over the coming days, I'll continue having cloud push new changes if you want to follow along with cloud's continued attempts to add by addressing these limitations.

## Evolution of language models, autonomous agent teams, and the future of software development with human oversight

  [Unknown]: Looking forward, each generation of language models opens up new ways of working with them.
  [Unknown]: Early models were useful for tab completion in IDE. Before long, models could complete the function body from its stock string.
  [Unknown]: The launch of cloud code brought agents into the mainstream and enabled developers to pair program with cloud, but each of these products operates under the assumption that a user defines a task.
  [Unknown]: An LLM runs for a few seconds or minutes and returns an answer, and then the user provides a follow-up.
  [Unknown]: Agent teams show that possibilities of implementing entire complex projects autonomously, this allow us as users of these tools to become more ambitious with our goals.
  [Unknown]: We are still early and fully autonomous development comes with real risks.
  [Unknown]: When a human sits with cloud during development, they can ensure consistent quality and catch errors in real time.

## Evolution of language models, autonomous agent teams, and the future of software development with human oversight

  [Unknown]: autonomous systems, it is easy to see tests pass and assume the job is done, when this is rarely the case. I used to work in penetration testing, exploiting vulnerabilities in products produced by large companies, and the thought of programmers deploying software they've never personally personally verified is a real concern. So, while this experiment excites me, it also leaves me feeling uneasy. Building this compiler has been some of the most fun I've recently, but I did not expect this to be anywhere near possible so early in 2026. The rapid progress in both language models and the scaffolds we use to interact with them opens the doors to writing an enormous amount of new code. I expect the positive applications to outweigh the negative, but we are entering a new world which will require new strategies to navigate safely.

## Acknowledgments for contributions to the article

  [Unknown]: acknowledgements, special thanks to Joseph Basic, Edwin Chen, Bernardo Meurer Costa, Jake Eaton, Dan Kelly, Felix Clock, Janet Park, Steve Weiss, and many other people across Anthropic for the assistance and contributions.

## Availability of the compiler, methodology for testing LLMs, and future development plans

  [Unknown]: Well, that's it.
  [Unknown]: We're going to open the compiler in GitHub.
  [Unknown]: We're going to mark it with a star.
  [Unknown]: We are gonna

## Miscellaneous brief remarks and interjections

  [Unknown]: of work.
  [Unknown]: Maybe the star.
  [Unknown]: Pana.

## General remarks on the future of AI agents and CLIs

  [Unknown]: pretty much anything you build today should come with a CLI for agents.
  [Unknown]: Agents are about to come from every single lab, not just Cloudbot.
