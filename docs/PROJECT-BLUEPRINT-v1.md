# MEDICA NOTICIA — Project Blueprint v1.0

## Documento Maestro para el Equipo de Construcción

### Fecha: Febrero 2026 | Preparado por: Project Management AI

-----

# TABLA DE CONTENIDOS

1. [Resumen Ejecutivo](#1-resumen-ejecutivo)
1. [Visión, Misión y Problema](#2-visión-misión-y-problema)
1. [Concepto Central: "Optimizar"](#3-concepto-central-optimizar)
1. [Audiencia Objetivo](#4-audiencia-objetivo)
1. [Sistema de Contenido: La Semana con Personalidad](#5-sistema-de-contenido-la-semana-con-personalidad)
1. [Categorías de Contenido](#6-categorías-de-contenido)
1. [Sistema Visual: Clasificación Floral por Mes](#7-sistema-visual-clasificación-floral-por-mes)
1. [Fuentes Internacionales](#8-fuentes-internacionales)
1. [Estructura de un Artículo](#9-estructura-de-un-artículo)
1. [Stack Técnico Definitivo](#10-stack-técnico-definitivo)
1. [Arquitectura del Backend](#11-arquitectura-del-backend)
1. [Esquema de Base de Datos (Supabase)](#12-esquema-de-base-de-datos-supabase)
1. [CMS y Flujo Editorial](#13-cms-y-flujo-editorial)
1. [Automatización con n8n](#14-automatización-con-n8n)
1. [Integraciones de IA y Audio](#15-integraciones-de-ia-y-audio)
1. [Frontend: Diseño y UX](#16-frontend-diseño-y-ux)
1. [SEO y Metadata](#17-seo-y-metadata)
1. [Sistema Multi-Agente (MAS)](#18-sistema-multi-agente-mas)
1. [Plan de Marketing](#19-plan-de-marketing)
1. [Plan Financiero](#20-plan-financiero)
1. [Roadmap de Desarrollo por Fases](#21-roadmap-de-desarrollo-por-fases)
1. [Asignación de Roles para los 5 Agentes](#22-asignación-de-roles-para-los-5-agentes)
1. [Riesgos y Mitigación](#23-riesgos-y-mitigación)
1. [Checklist de Lanzamiento MVP](#24-checklist-de-lanzamiento-mvp)
1. [Apéndices y Referencias Técnicas](#25-apéndices-y-referencias-técnicas)

-----

# 1. RESUMEN EJECUTIVO

Medica Noticia (www.medicanoticia.com) es una revista digital especializada en noticias médicas y de salud positivas, validadas y accesibles. La plataforma cura y "optimiza" contenido de fuentes internacionales confiables de todos los continentes, lo traduce al español y lo presenta en un formato claro, artístico, sin anuncios, y gratuito.

Lo que construimos: Una plataforma web completa con generación de contenido asistida por IA, revisión humana (human-in-the-loop), distribución multicanal, audio text-to-speech, chatbot interactivo, y búsqueda semántica avanzada.

Lo que NO es: Un agregador automático sin supervisión. Todo contenido pasa por revisión editorial humana antes de publicarse.

Modelo: Semi-automatizado — la IA genera y sugiere, el humano revisa y aprueba.

-----

# 2. VISIÓN, MISIÓN Y PROBLEMA

## Misión

> "Hacer que la información médica sea accesible y fácil de entender para todos, optimizando y resumiendo contenido de las mejores fuentes internacionales traducidas al español, para que cada persona pueda tomar decisiones informadas sobre su salud."

## Visión

> "Convertirnos en la principal fuente de información médica en español, empoderando a las personas con conocimiento claro, confiable y accesible, que mejore su bienestar y calidad de vida."

## El Problema que Resolvemos

Existe un alto grado de contaminación en el espacio de noticias médicas y salud pública. Intereses comerciales agravan la desinformación, generando caos, miedo, incertidumbre y problemas sociales. Las noticias alarmistas y fuera de contexto generan ansiedad, estrés, adicciones, desconfianza y enfermedad.

## Nuestra Solución

Médica Noticia actúa como mediador y curador de noticias de fuentes cuidadosamente seleccionadas, presentadas de manera recurrente, clara y transparente. Alimentamos el ecosistema digital con información positiva, proporcionando un espacio de armonía, calma y esperanza, ofreciendo profundidad y veracidad en las fuentes.

-----

# 3. CONCEPTO CENTRAL: "OPTIMIZAR"

Para Medica Noticia, "optimizar" significa:

1. Seleccionar los mejores artículos médicos de fuentes confiables de todo el mundo
1. Resumir de manera concisa y positiva
1. Traducir al español manteniendo precisión médica
1. Presentar con arte, diseño minimalista y accesibilidad
1. Ofrecer audio de los artículos para máxima comodidad
1. Mantener transparencia total — cada fuente utilizada se publica íntegramente y es visible durante toda la experiencia del usuario

Principio clave: Si algo te llama la atención, siempre puedes acceder al artículo completo original con un simple clic.

Cada fuente tiene su propia página de transparencia: www.medicanoticia.com/nuestrasfuentes/transparencia/

-----

# 4. AUDIENCIA OBJETIVO

## Audiencia Primaria

- Profesionales de la salud hispanohablantes — médicos, enfermeras, investigadores que necesitan resúmenes rápidos y confiables de avances médicos globales.

## Audiencia Secundaria

- Público general hispanohablante interesado en temas médicos — desde un adulto mayor hasta cualquier persona que quiera tomar decisiones informadas sobre su salud.

## Mercados Geográficos

- España, México, Colombia, Argentina, Chile, Puerto Rico, y toda Latinoamérica
- Comunidades hispanohablantes en EE.UU.
- Expansión futura a contenido en inglés (Fase 3)

-----

# 5. SISTEMA DE CONTENIDO: LA SEMANA CON PERSONALIDAD

Medica Noticia sigue un ciclo concéntrico que se despliega desde el interior hacia el exterior, adaptándose a la naturaleza semanal de cada día. Cada día tiene una personalidad propia que define el tono, temática, energía y color del contenido publicado.

## Estructura Semanal Completa

### 🔵 LUNES — Día del Yo (Self-Care y Bienestar Interno)

- Temática: Salud mental y emocional, mejora personal
- Contenido: Noticias sobre el cerebro, mindfulness, anatomía interna, gestión del estrés
- Energía: Reflexiva y enfocada en el cuidado personal
- Color: #87CEEB Azul Celeste
- Tono editorial: Introspectivo, sereno y empático. Invitar a una pausa mental
- Actividades del equipo: Revisión del sitio web, creación de contenido, reunión de equipo
- Ejemplo de artículo: "Técnicas de mindfulness para comenzar la semana con mente equilibrada"

### 🟡 MARTES — Día del Trabajo (Vida Laboral y Salud Ocupacional)

- Temática: Innovación y descubrimientos en el ámbito laboral
- Contenido: Avances en medicina, ergonomía, tecnologías laborales, salud ocupacional
- Energía: Proactiva y enfocada en la eficiencia laboral
- Color: #FFD700 Amarillo
- Tono editorial: Motivador, innovador, orientado a soluciones
- Actividades del equipo: Revisión de fuentes, creación de arte, brainstorming

### 🟢 MIÉRCOLES — Día de la Salud Física

- Temática: Bienestar físico y ejercicio
- Contenido: Noticias sobre fitness, nutrición, importancia del sueño, deporte y salud
- Energía: Energética y vital
- Color: #00CC00 Verde
- Tono editorial: Activo, motivador, práctico
- Actividades del equipo: Revisión de contenido, actualización de redes sociales

### 🟠 JUEVES — Día de la Salud Social

- Temática: Relaciones y vida social
- Contenido: Salud comunitaria, impacto social en la salud, relaciones interpersonales
- Energía: Social y comunitaria
- Color: #FF8C00 Naranja
- Tono editorial: Cálido, comunitario, empático
- Actividades del equipo: Revisión de la web, creación de arte, discusión sobre impacto social

### 🔴 VIERNES — Día del Mundo y la Actualidad

- Temática: Noticias internacionales y salud global
- Contenido: Salud pública, eventos médicos globales, investigaciones internacionales
- Energía: Extrovertida y global
- Color: #FF0000 Rojo
- Tono editorial: Informativo, global, actual
- Actividades del equipo: Revisión de fuentes, actualización de redes sociales

### 🟣 SÁBADO — Día de la Preparación y Protección

- Temática: Planificación y protección personal
- Contenido: Estrategias de prevención, meditación, relajación, preparación para la salud
- Energía: Reflexiva y protectora
- Color: #800080 Morado
- Tono editorial: Preventivo, protector, planificador
- Actividades del equipo: Revisión de contenido, creación de arte, planificación semanal

### ⚪ DOMINGO — Día del Reposo y el Cuidado

- Temática: Descanso y cuidado integral
- Contenido: Tecnologías de salud, dispositivos de seguimiento, bienestar integral
- Energía: Calmante y restaurativa
- Color: #FFFFFF Blanco
- Tono editorial: Tranquilo, restaurativo, tecnológico pero accesible
- Actividades del equipo: Revisión de la web, actualización de redes sociales

-----

# 6. CATEGORÍAS DE CONTENIDO

Todo artículo publicado en Medica Noticia pertenece a una de estas 5 categorías principales:

| # | Categoría | Descripción | Ejemplo de Temas |
|---|-----------|-------------|------------------|
| 1 | **Actualidad** | Noticias médicas recientes y eventos de salud global | Brotes, políticas de salud, conferencias médicas |
| 2 | **Bienestar** | Salud integral, prevención y calidad de vida | Mindfulness, nutrición, ejercicio, sueño |
| 3 | **Descubrimiento** | Nuevos hallazgos científicos y avances en investigación | Estudios clínicos, nuevas terapias, genómica |
| 4 | **Tecnología** | Innovaciones tecnológicas aplicadas a la salud | IA en diagnóstico, wearables, telemedicina |
| 5 | **Mundo** | Perspectiva global de salud por regiones y continentes | Salud en Asia, avances en Europa, salud en África |

Relación Categoría-Día: Si bien cualquier categoría puede publicarse cualquier día, existe una afinidad natural:

- Lunes → Bienestar
- Martes → Tecnología / Descubrimiento
- Miércoles → Bienestar (físico)
- Jueves → Actualidad (social)
- Viernes → Mundo / Actualidad
- Sábado → Bienestar (prevención)
- Domingo → Tecnología

-----

# 7. SISTEMA VISUAL: CLASIFICACIÓN FLORAL POR MES

Cada mes tiene dos flores principales que rotan diariamente como elemento visual del arte de portada. Este sistema asegura coherencia estética y resonancia temática estacional.

| Mes | Tema | Flor 1 | Flor 2 |
|-----|------|--------|--------|
| **Enero** | Nuevos Comienzos | Clavel (*Dianthus caryophyllus*) | Campanilla de invierno (*Galanthus nivalis*) |
| **Febrero** | Amor y Amistad | Violeta (*Viola spp.*) | Prímula (*Primula vulgaris*) |
| **Marzo** | Nuevo Crecimiento | Narciso (*Narcissus pseudonarcissus*) | Jonquil (*Narcissus jonquilla*) |
| **Abril** | Primavera en Flor | Margarita (*Bellis perennis*) | Guisante de olor (*Lathyrus odoratus*) |
| **Mayo** | Floración y Vitalidad | Lirio de los valles (*Convallaria majalis*) | Espino (*Crataegus spp.*) |
| **Junio** | Calidez y Alegría | Rosa (*Rosa spp.*) | Madreselva (*Lonicera spp.*) |
| **Julio** | Esplendor de Verano | Nenúfar (*Nymphaea spp.*) | Delfinio (*Delphinium spp.*) |
| **Agosto** | Abundancia y Cosecha | Gladiolo (*Gladiolus spp.*) | Amapola (*Papaver spp.*) |
| **Septiembre** | Transición y Cambio | Aster (*Aster spp.*) | Gloria de la mañana (*Ipomoea spp.*) |
| **Octubre** | Gloria de Otoño | Caléndula (*Tagetes spp.*) | Cosmos (*Cosmos bipinnatus*) |
| **Noviembre** | Reflexión y Gratitud | Crisantemo (*Chrysanthemum spp.*) | Poinsettia (*Euphorbia pulcherrima*) |
| **Diciembre** | Festivo y Acogedor | Acebo (*Ilex spp.*) | Narciso (*Narcissus tazetta*) |

Rotación diaria: Día 1 = Flor 1, Día 2 = Flor 2, repetir patrón.

Uso en el arte de portada: Cada artículo genera una imagen de portada con DALL-E 3 que integra sutilmente la flor del día y el color del día de la semana.

-----

# 8. FUENTES INTERNACIONALES

Medica Noticia cura contenido de fuentes de todos los continentes (excepto Antártida). La transparencia de fuentes es un pilar fundamental.

## Asia

1. The Lancet Asia — Investigaciones clave en salud en Asia
1. BMJ Asia — Investigaciones relevantes para la región asiática
1. The Indian Journal of Medical Research — Fuente importante en India
1. Chinese Medical Journal — Revista oficial de la Asociación Médica China

## África

1. The African Journal of Primary Health Care & Family Medicine — Atención primaria
1. South African Medical Journal — Una de las más influyentes de África
1. Pan African Medical Journal — Investigaciones de todo el continente

## América del Norte

1. The New England Journal of Medicine (NEJM) — Una de las más influyentes a nivel mundial
1. JAMA (Journal of the American Medical Association) — Investigaciones fundamentales
1. CMAJ (Canadian Medical Association Journal) — Principal revista de Canadá

## América del Sur

1. Revista Médica de Chile — Una de las más antiguas y respetadas
1. Cadernos de Saúde Pública — Salud pública en Brasil
1. Revista Panamericana de Salud Pública — OPS, cubre toda América Latina

## Europa

1. The Lancet — Origen UK, alcance global
1. BMJ (British Medical Journal) — Una de las más prestigiosas
1. European Journal of Clinical Investigation — Alta calidad en Europa

## Oceanía

1. The Medical Journal of Australia (MJA) — Principal de Australia
1. New Zealand Medical Journal (NZMJ) — Principal de Nueva Zelanda
1. Pacific Health Dialog — Islas del Pacífico y Oceanía

Página de transparencia: Cada fuente tiene su propia página accesible permanentemente en: www.medicanoticia.com/nuestrasfuentes/transparencia/

-----

# 9. ESTRUCTURA DE UN ARTÍCULO

Cada artículo publicado en Medica Noticia debe contener estos campos:

## Campos Obligatorios

| Campo | Tipo | Especificaciones |
|-------|------|------------------|
| **Título** | VARCHAR(100) | Conciso y atractivo, máximo 100 caracteres |
| **Resumen** | TEXT | Entre 150-450 palabras |
| **Categoría** | UUID → Categories | Una de las 5 categorías principales |
| **Contenido** | TEXT | 1000-1500 palabras (estándar) / hasta 3000 (profundidad) |
| **Autor** | UUID → Users | Vinculado a tabla de usuarios |
| **Palabras Clave** | ARRAY | 5-8 keywords relevantes |
| **Referencias** | TEXT | Formato APA, máximo 10 referencias |
| **Meta Descripción** | VARCHAR(160) | 150-160 caracteres para SEO |
| **Keyword Principal** | VARCHAR | Palabra clave principal para SEO |
| **Keywords Relacionadas** | ARRAY | 3-5 palabras clave adicionales |
| **Fecha de Publicación** | TIMESTAMP | Fecha y hora programada |
| **Estado** | ENUM | draft / review / approved / published |
| **Sensibilidad Temporal** | ENUM | timely / evergreen |

## Campos Opcionales

| Campo | Tipo | Especificaciones |
|-------|------|------------------|
| **Elementos Multimedia** | TEXT | Descripción de diagramas/infografías (máx 50 palabras c/u) |
| **Artículos Relacionados** | UUID[] | 2-3 artículos existentes para vincular |
| **Perspectivas de Expertos** | TEXT | Nombres y credenciales de expertos consultados |
| **Temas de Seguimiento** | TEXT | 2-3 ideas para futuros artículos |
| **Archivo de Audio** | URL | Enlace al audio generado por ElevenLabs |
| **Cover Art** | URL | Imagen de portada generada por DALL-E 3 |

## Requisitos Técnicos del Contenido

- Formato: Markdown (.md) o texto plano (.txt)
- Imágenes: .jpg o .png, mínimo 1200x800px, máximo 2MB
- Estructura: H2 para secciones principales, H3 para subsecciones
- Codificación: UTF-8
- Nomenclatura: AAAA-MM-DD_Titulo-del-Articulo.md
- Tono: Positivo, validado, accesible
- Idioma: Español (expansión a inglés en Fase 3)
- Frecuencia: 3-5 artículos por semana
- Revisiones: Hasta 2 rondas basadas en comentarios del editor

-----

# 10. STACK TÉCNICO DEFINITIVO

## Capa de Presentación (Frontend)

| Componente | Tecnología | Propósito |
|------------|-----------|-----------|
| Framework | **React + Next.js** | UI dinámica con SSR para SEO |
| Estilos | **Tailwind CSS** | Diseño responsivo y minimalista |
| Componentes UI | **shadcn/ui + Custom** | Componentes accesibles y consistentes |
| Iconos | **Lucide React** | Iconografía consistente |
| Estado | **React Context API** | Gestión de estado (Redux para complejidad futura) |
| Visualización de grafos | **D3.js o Cytoscape.js** | Relaciones entre contenido |

## Capa de Datos (Backend)

| Componente | Tecnología | Propósito |
|------------|-----------|-----------|
| Base de datos primaria | **Supabase (PostgreSQL)** | Datos relacionales, auth, real-time |
| Base de datos de grafos | **Neo4j AuraDB** | Relaciones complejas entre entidades |
| Búsqueda | **Elasticsearch** | Búsqueda avanzada de contenido |
| Búsqueda semántica | **Qdrant o Pinecone** | Vector DB para búsqueda por significado |
| CMS | **Strapi (Headless)** | Gestión de contenido editorial |
| API | **GraphQL (Apollo) + REST** | Capa de datos para el frontend |

## Capa de IA y Audio

| Componente | Tecnología | Propósito |
|------------|-----------|-----------|
| Generación de contenido | **OpenAI API (GPT-4)** | Resúmenes, traducciones, optimización |
| Generación de imágenes | **DALL-E 3** | Cover art con sistema floral |
| Text-to-Speech | **ElevenLabs** | Audio de artículos en español |
| Chatbot | **Dialogflow o Rasa** | Asistente interactivo para usuarios |
| Speech-to-Text (futuro) | **Deepgram** | Transcripción de audio |

## Capa de Infraestructura

| Componente | Tecnología | Propósito |
|------------|-----------|-----------|
| Hosting | **Vercel** | Deployment continuo del frontend |
| Contenedores | **Docker** | Entornos consistentes de desarrollo |
| Automatización | **n8n** | Workflows entre todas las herramientas |
| Gestión de proyecto | **Notion** | Hub central de coordinación |
| CRM | **GoHighLevel** | Gestión de relaciones y marketing |
| Versionamiento | **GitHub** | Control de código fuente |
| Monitoreo | **Sentry + Supabase Dashboard** | Errores y performance |

## Integraciones Adicionales

| Herramienta | Uso |
|-------------|-----|
| **Google Drive** | Almacenamiento de assets y documentos |
| **Google Docs** | Colaboración en borradores |
| **Airtable** | Base de datos flexible para tracking de fuentes |
| **X (Twitter)** | Distribución de contenido social |

-----

# 11. ARQUITECTURA DEL BACKEND

## Diagrama de Arquitectura

```
┌─────────────────────────────────────────────────────────┐
│                       USUARIOS                          │
│                (Web Browser / Mobile)                    │
└──────────────────────┬──────────────────────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────────────────────┐
│                  FRONTEND (Vercel)                       │
│            React + Next.js + Tailwind CSS               │
│               SSR/SSG para SEO óptimo                   │
└──────────────────────┬──────────────────────────────────┘
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
┌──────────────┐ ┌──────────┐ ┌──────────────┐
│   Supabase   │ │  Strapi  │ │    Neo4j     │
│  PostgreSQL  │ │   CMS    │ │   AuraDB     │
│  Auth + RLS  │ │ Headless │ │  Graph DB    │
│  Real-time   │ │          │ │              │
└──────┬───────┘ └────┬─────┘ └──────┬───────┘
       │              │              │
       └──────────────┼──────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────┐
│                    n8n (Docker)                          │
│               Workflow Automation Hub                    │
│                                                         │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐  │
│  │  OpenAI  │ │ElevenLabs│ │  Notion  │ │  DALL-E  │  │
│  │  GPT-4   │ │   TTS    │ │   API    │ │    3     │  │
│  └──────────┘ └──────────┘ └──────────┘ └──────────┘  │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐  │
│  │  GoHigh  │ │  Google  │ │ Airtable │ │X/Twitter │  │
│  │  Level   │ │  Drive   │ │          │ │   API    │  │
│  └──────────┘ └──────────┘ └──────────┘ └──────────┘  │
└─────────────────────────────────────────────────────────┘
```

## Enfoque Semi-Automatizado

El sistema usa un modelo Human-in-the-Loop donde:

1. n8n automatiza la generación y sincronización inicial de contenido
1. El equipo editorial revisa y edita el contenido en Notion/Strapi antes de publicación
1. n8n automatiza la publicación final y distribución multicanal
1. El feedback de usuarios se registra automáticamente para análisis

-----

# 12. ESQUEMA DE BASE DE DATOS (SUPABASE)

## Tablas Principales

### Users (Usuarios)

```sql
CREATE TABLE users (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    email VARCHAR(255) UNIQUE NOT NULL,
    password_hash VARCHAR(255) NOT NULL,
    full_name VARCHAR(255),
    role VARCHAR(50) NOT NULL DEFAULT 'reader',
    avatar_url TEXT,
    created_at TIMESTAMP DEFAULT now(),
    updated_at TIMESTAMP DEFAULT now()
);
```

### Categories (Categorías)

```sql
CREATE TABLE categories (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    name VARCHAR(100) NOT NULL,
    slug VARCHAR(100) UNIQUE NOT NULL,
    description TEXT,
    color VARCHAR(7),
    icon VARCHAR(50),
    created_at TIMESTAMP DEFAULT now(),
    updated_at TIMESTAMP DEFAULT now()
);
```

### Articles (Artículos)

```sql
CREATE TABLE articles (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    title VARCHAR(100) NOT NULL,
    slug VARCHAR(200) UNIQUE NOT NULL,
    summary TEXT NOT NULL,
    content TEXT NOT NULL,
    category_id UUID REFERENCES categories(id),
    author_id UUID REFERENCES users(id),
    source_url TEXT,
    source_name VARCHAR(255),
    cover_image_url TEXT,
    audio_url TEXT,
    meta_description VARCHAR(160),
    primary_keyword VARCHAR(100),
    related_keywords TEXT[],
    day_of_week VARCHAR(20),
    day_color VARCHAR(7),
    month_flower VARCHAR(100),
```

*[DOCUMENTO INCOMPLETO — Continuación pendiente]*
