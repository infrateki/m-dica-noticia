# Médica Noticia — Complete Miro Board Specs

*Full technical export from Miro board — February 8, 2026*
*Original work by Sergio & Daniela (~2024)*

---

## Homepage Wireframe

### Boceto de la Página de Inicio:

1. **Encabezado:**
   - Parte superior izquierda: Logo (Médica Noticia)
   - Parte superior derecha: Cambiador de idioma (ES/EN), ícono de búsqueda, ícono de cuenta de usuario
   - Debajo: Menú de navegación principal (Inicio, Actualidad, Bienestar, Descubrimiento, Tecnología, Mundo, Chat Médico)

2. **Sección Hero:**
   - Artículo destacado grande con imagen llamativa, título, breve descripción, botón "Leer más"

3. **Barra de búsqueda:**
   - Prominente a todo lo ancho debajo de la sección hero
   - Placeholder: "Buscar artículos, temas o autores"

4. **Categorías destacadas:**
   - Diseño en cuadrícula 3-4 columnas
   - Cada categoría: Ícono, nombre, breve descripción

5. **Últimos artículos:**
   - Grid 3 columnas (2 tabletas, 1 móviles)
   - Tarjeta: imagen, título, extracto, categoría, tiempo de lectura

6. **Newsletter:**
   - Sección a todo lo ancho: "Mantente Informado"
   - Campo email + botón "Suscribirse"

7. **Chat Médico:**
   - Botón flotante esquina inferior derecha
   - Ícono de profesional médico / burbuja de chat

8. **Pie de página:**
   - Logo, descripción, enlaces, redes sociales, copyright

### UX Notes from Miro:
- "la imagen es blurry de primera vista pero si le das click se ve el arte"
- "Siempre se ve el arte sin ser opaco, pero las imágenes siguen la estructura o línea de color de cada día: Lunes (azul), Martes (verde)..."
- "CADA MES TIENE ESTA CON HECHO CON UN ESTILO DIFERENTE"

---

## Project Overview

Médica Noticia (www.medicanoticia.com) is a digital magazine specializing in providing positive, validated, and accessible medical and health news.

**Brand:** "Positive, transparent, succinct, readable, listenable, premium, most relevant, breaking news"

### Mission
"To make medical information accessible and easy to understand for everyone, by optimizing and summarizing content into 200-450 words summaries from the best sources from 5 continents."

### Vision
"To become the main source of medical information in Spanish, empowering people with clear, reliable, and accessible knowledge."

---

## Core Features

1. **Persistent Search/Chat Bar** — Always-accessible, leveraging GraphRAG
2. **Curated Articles** — 5 categories, daily updates with weekly mood themes
3. **AI-Powered Content** — OpenAI + Anthropic for curation, generation, summarization
4. **Audio Content** — TTS for all articles, male/female voices, ES/EN
5. **Advanced Search** — Elasticsearch with faceted search
6. **Responsive Design** — Mobile-first
7. **Analytics** — shadcn integration
8. **Related Articles** — Graph-based recommendations
9. **Multilingual** — ES/EN initially, extensible

---

## Development Phases

### Phase 3: Content Management and Data Integration
- Strapi CMS integration
- Neo4j AuraDB + Supabase integration
- GraphQL API for graph-based queries
- Basic GraphRAG functionality

### Phase 4: AI Integration and Advanced Search
- OpenAI content generation/summarization
- ElevenLabs TTS
- AI-powered recommendations
- Interactive "Knowledge Explorer"

### Phase 5: UI/UX Refinement (Weeks 21-26)
- Responsive design refinement
- Animations and transitions
- User testing
- Advanced filtering with graph properties
- Personalized dashboards with knowledge graphs
- Third-party integrations: flowise.ai, mindstudio, bubble

---

## Frontend Flowchart (Excalidraw)

### Content Creator Machine Frontend Structure

**Overall Structure and Design** → Main Components:
- Header Component (Logo, Navigation, Language switcher, Dark mode, Search/Chat bar)
- Dashboard Component (Content status, Weekly theme, Category access)
- ContentPipeline Component (Creation process visualization, Status updates)
- CategoryManager Component (Actualidad, Bienestar, Descubrimiento, Tecnología, Mundo)
- WeeklyCycle Component (Calendar view, Theme settings per day)
- AIIntegration Component (OpenAI/Anthropic settings, Customization)
- SourceManager Component (RSS feeds, Feedly integration)
- PublishingQueue Component (Review/approval, Direct publishing)
- Analytics Component (Performance metrics, Engagement stats, AI analysis)

**Workflow Integration:**
- Connect with Make.com and Zapier
- Integrate with Google Docs
- Implement Notion API

**Content Creation Process:**
Source Aggregation → AI Processing → Translation → Human Review → Publishing

**Weekly Cycle Implementation:**
- Monday: "Actualidad" focus
- Tuesday: "Bienestar" focus
- Wednesday: "Descubrimiento" focus
- Thursday: "Tecnología" focus
- Friday: "Mundo" focus
- Weekend: Mix of all categories

**Flower Art Concept Integration:**
- Use flower motif throughout UI
- "Content Garden" visualization
- Color-code flowers based on categories

---

## Original Project Structure (Next.js)

```
medica-noticia/
├── pages/
│   ├── _app.tsx
│   ├── _document.tsx
│   ├── index.tsx
│   ├── actualidad.tsx
│   ├── bienestar.tsx
│   ├── descubrimiento.tsx
│   ├── tecnologia.tsx
│   ├── mundo.tsx
│   ├── chat.tsx
│   ├── articulos/
│   │   └── [slug].tsx
│   └── api/
│       ├── articles.ts
│       ├── search.ts
│       ├── chat.ts
│       └── auth.ts
├── components/
│   ├── layout/ (Layout, Header, Footer)
│   ├── ui/ (Button, Card, SearchBar)
│   ├── home/ (HeroSection, NewsSection, WellbeingSection)
│   ├── articles/ (ArticleCard, ArticleContent, RelatedArticles)
│   └── chat/ (ChatInterface, MessageList, MessageInput, BotResponse)
├── lib/ (supabase.ts, neo4j.ts, openai.ts, elevenlabs.ts)
├── hooks/ (useArticles.ts, useChat.ts)
├── contexts/ (AuthContext.tsx)
├── styles/ (globals.css)
├── types/ (index.ts)
├── utils/ (helpers.ts)
└── public/images/
```

---

## Pipeline Notes from Miro

```
NOTION/PLAN DE CONTENIDO → RSS/FUENTES → NOTICIA RELEVANTE →
OPENAI CREACIÓN ARTÍCULO POST → OPTIMIZACIÓN SEO → MIRO →
MIDJOURNEY (imagen acorde a specs del día) → DOCUMENTO MS WORD →
NOTION/GOOGLE SHEET → SE PUBLICA EN WORDPRESS → SM (X, Instagram, Facebook)
```

**Key questions noted in Miro:**
- "¿ES LAS DOS EN UNA??" (regarding source + article generation)
- "¿EN QUE MOMENTO SE REVISA SI LA INFORMACIÓN GENERADA ES CORRECTA?"
- "¿AQUI EXTRAE LA IMAGEN?"

**Automation tools noted:** Make.com, webhooks, RSS feeds, Google Analytics

---

*NOTE: The tech stack documented here (Next.js, Strapi, WordPress) is from 2024 and considered OBSOLETE by Sergio as of Feb 2026. The new architecture will be agent-native (see reference articles in docs/references/). The SOUL of the project (mission, vision, art, content system) remains unchanged.*
