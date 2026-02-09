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
    is_evergreen BOOLEAN DEFAULT false,
    reading_time_minutes INTEGER,
    status VARCHAR(20) NOT NULL DEFAULT 'draft',
    published_at TIMESTAMP,
    created_at TIMESTAMP DEFAULT now(),
    updated_at TIMESTAMP DEFAULT now()
);
```

### Tags (Etiquetas)

```sql
CREATE TABLE tags (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    name VARCHAR(100) UNIQUE NOT NULL,
    slug VARCHAR(100) UNIQUE NOT NULL,
    created_at TIMESTAMP DEFAULT now()
);

CREATE TABLE article_tags (
    article_id UUID REFERENCES articles(id) ON DELETE CASCADE,
    tag_id UUID REFERENCES tags(id) ON DELETE CASCADE,
    PRIMARY KEY (article_id, tag_id)
);
```

### References (Fuentes y Citas)

```sql
CREATE TABLE article_references (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    article_id UUID REFERENCES articles(id) ON DELETE CASCADE,
    citation_text TEXT NOT NULL,
    source_url TEXT,
    source_name VARCHAR(255),
    continent VARCHAR(50),
    order_index INTEGER,
    created_at TIMESTAMP DEFAULT now()
);
```

### Publication Schedule (Horario de Publicación)

```sql
CREATE TABLE publication_schedule (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    article_id UUID REFERENCES articles(id) ON DELETE CASCADE,
    publish_date DATE NOT NULL,
    publish_time TIME,
    social_media_scheduled BOOLEAN DEFAULT false,
    newsletter_scheduled BOOLEAN DEFAULT false,
    created_at TIMESTAMP DEFAULT now(),
    updated_at TIMESTAMP DEFAULT now()
);
```

### Feedback (Retroalimentación)

```sql
CREATE TABLE feedback (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    article_id UUID REFERENCES articles(id) ON DELETE CASCADE,
    user_id UUID REFERENCES users(id),
    comment TEXT,
    rating INTEGER CHECK (rating >= 1 AND rating <= 5),
    created_at TIMESTAMP DEFAULT now()
);
```

### Comments (Comentarios)

```sql
CREATE TABLE comments (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    article_id UUID REFERENCES articles(id) ON DELETE CASCADE,
    user_id UUID REFERENCES users(id),
    parent_id UUID REFERENCES comments(id),
    content TEXT NOT NULL,
    is_approved BOOLEAN DEFAULT false,
    created_at TIMESTAMP DEFAULT now(),
    updated_at TIMESTAMP DEFAULT now()
);
```

### User Interactions (Interacciones)

```sql
CREATE TABLE favorites (
    user_id UUID REFERENCES users(id) ON DELETE CASCADE,
    article_id UUID REFERENCES articles(id) ON DELETE CASCADE,
    created_at TIMESTAMP DEFAULT now(),
    PRIMARY KEY (user_id, article_id)
);

CREATE TABLE reading_history (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    user_id UUID REFERENCES users(id) ON DELETE CASCADE,
    article_id UUID REFERENCES articles(id) ON DELETE CASCADE,
    read_at TIMESTAMP DEFAULT now(),
    reading_duration_seconds INTEGER
);

CREATE TABLE subscriptions (
    id UUID PRIMARY KEY DEFAULT uuid_generate_v4(),
    user_id UUID REFERENCES users(id) ON DELETE CASCADE,
    plan_name VARCHAR(50) NOT NULL,
    start_date DATE NOT NULL,
    end_date DATE,
    is_active BOOLEAN DEFAULT true,
    created_at TIMESTAMP DEFAULT now()
);
```

## Relaciones (Diagrama ER)

```
Users ──┬── 1:N ──→ Articles
        ├── 1:N ──→ Comments
        ├── 1:N ──→ Feedback
        ├── N:N ──→ Favorites ←── Articles
        └── 1:N ──→ Subscriptions

Categories ── 1:N ──→ Articles

Articles ──┬── 1:N ──→ Comments
           ├── 1:N ──→ Feedback
           ├── 1:N ──→ Article_References
           ├── N:N ──→ Article_Tags ←── Tags
           └── 1:1 ──→ Publication_Schedule
```

## Row Level Security (RLS)

```sql
ALTER TABLE articles ENABLE ROW LEVEL SECURITY;

CREATE POLICY "Public read published" ON articles
    FOR SELECT USING (status = 'published');

CREATE POLICY "Editors can insert" ON articles
    FOR INSERT WITH CHECK (auth.role() IN ('editor', 'admin'));

CREATE POLICY "Editors can update" ON articles
    FOR UPDATE USING (auth.role() IN ('editor', 'admin'));

CREATE POLICY "Admins can delete" ON articles
    FOR DELETE USING (auth.role() = 'admin');
```

-----

# 13. CMS Y FLUJO EDITORIAL

## Flujo de Contenido Completo

```
1. SOURCING → n8n monitorea fuentes RSS/APIs de journals médicos
   ↓
2. AI GENERATION → OpenAI genera resumen + traducción + keywords
   ↓
3. DRAFT → Artículo se crea en Supabase (status: draft)
   ↓
4. SYNC TO NOTION → n8n sincroniza a Notion Content Tracker
   ↓
5. EDITORIAL REVIEW → Editor humano revisa en Notion/Strapi
   ↓
6. APPROVAL → Editor cambia status a "approved"
   ↓
7. MEDIA GENERATION → n8n dispara:
   • DALL-E 3 genera cover art (flor del mes + color del día)
   • ElevenLabs genera audio del artículo
   ↓
8. PUBLICATION → n8n publica en el frontend (status: published)
   ↓
9. DISTRIBUTION → n8n distribuye a:
   • X/Twitter (social card)
   • Newsletter (GoHighLevel)
   • RSS Feed
   ↓
10. MONITORING → Analytics tracean engagement y feedback
```

## Strapi CMS Configuration

Strapi actúa como el CMS headless donde el equipo editorial puede:

- Crear y editar artículos con editor visual rico
- Gestionar categorías y tags
- Programar publicaciones
- Gestionar multimedia
- Configurar workflows de aprobación

-----

# 14. AUTOMATIZACIÓN CON N8N

## Workflows Principales

### Workflow 1: Content Sync (Supabase → Notion)

- Trigger: New/Updated Row en tabla articles
- Action: Create/Update Page en Notion Content Tracker
- Mapping: title → Title, summary → Summary, category_id → Category, status → Status

### Workflow 2: Content Generation (Scheduled)

- Trigger: Cron (diario)
- Actions:
  1. HTTP Request a fuentes RSS de journals médicos
  1. OpenAI API para generar resumen + traducción
  1. Insert en Supabase tabla articles (status: draft)
  1. Notion sync automático

### Workflow 3: Media Generation (On Approval)

- Trigger: Article status cambia a "approved"
- Actions:
  1. DALL-E 3: Genera cover art con prompt que incluye flor del mes + color del día
  1. ElevenLabs: Genera audio del resumen del artículo
  1. Update article con URLs de media
  1. Cambiar status a "published"

### Workflow 4: Social Distribution (On Publish)

- Trigger: Article status cambia a "published"
- Actions:
  1. Generar social card optimizada para X/Twitter
  1. Publicar en X vía API
  1. Agregar a newsletter queue en GoHighLevel
  1. Notificar equipo vía Slack/Email

### Workflow 5: Feedback Integration (Supabase → Notion)

- Trigger: New Row en tabla feedback
- Action: Create Page en Notion Feedback Management

### Workflow 6: Weekly Analytics Report

- Trigger: Cron (cada lunes)
- Actions:
  1. Query Supabase para métricas de la semana
  1. Generar reporte con OpenAI
  1. Enviar a Notion y por email al equipo

## Docker Setup para n8n

```yaml
# docker-compose.yml
n8n:
  image: n8nio/n8n
  ports:
    - "5678:5678"
  environment:
    - N8N_BASIC_AUTH_ACTIVE=true
    - N8N_BASIC_AUTH_USER=admin
    - N8N_BASIC_AUTH_PASSWORD=secure_password_here
    - N8N_HOST=localhost
    - N8N_PORT=5678
    - N8N_PROTOCOL=http
    - NODE_ENV=production
  volumes:
    - n8n_data:/root/.n8n
```

## Environment Variables Necesarias

```bash
# Supabase
SUPABASE_URL=https://your-project.supabase.co
SUPABASE_KEY=your-supabase-key
SUPABASE_SERVICE_ROLE_KEY=your-service-role-key

# OpenAI
OPENAI_API_KEY=sk-your-openai-key

# ElevenLabs
ELEVENLABS_API_KEY=your-elevenlabs-key

# Notion
NOTION_TOKEN=your-notion-integration-token
NOTION_CONTENT_DB_ID=your-content-tracker-db-id
NOTION_FEEDBACK_DB_ID=your-feedback-db-id

# Strapi
STRAPI_URL=http://localhost:1337
STRAPI_API_TOKEN=your-strapi-token

# X/Twitter
TWITTER_API_KEY=your-twitter-key
TWITTER_API_SECRET=your-twitter-secret
TWITTER_ACCESS_TOKEN=your-access-token
TWITTER_ACCESS_SECRET=your-access-secret

# GoHighLevel
GHL_API_KEY=your-gohighlevel-key
```

-----

# 15. INTEGRACIONES DE IA Y AUDIO

## OpenAI — Generación de Contenido

### Prompt de Generación de Artículos

```
Eres un experto médico redactando para Medica Noticia, una revista digital en español.

Tu tarea es optimizar el siguiente artículo médico:

FUENTE ORIGINAL: [URL/texto del artículo]

INSTRUCCIONES:
1. Genera un título conciso y atractivo (máximo 100 caracteres)
2. Escribe un resumen de 150-450 palabras
3. Desarrolla el contenido completo (1000-1500 palabras)
4. El tono debe ser: [personalidad del día]
5. Categoría: [una de las 5 categorías]
6. Genera 5-8 palabras clave relevantes
7. Escribe una meta descripción SEO (150-160 caracteres)
8. Sugiere 2-3 artículos relacionados potenciales
9. Todo en español, accesible tanto para profesionales de salud como público general
10. Tono positivo, validado y esperanzador — NO alarmista

FORMATO DE SALIDA: JSON estructurado
```

### Prompt de Cover Art (DALL-E 3)

```
Crea una imagen de portada para un artículo médico sobre '[TÍTULO]'.

La imagen debe tener:
- Estética limpia médica/salud con [COLOR DEL DÍA] como color dominante
- Integración sutil y natural de flores de [FLOR DEL MES]
- Estilo minimalista, moderno y profesional
- Tono visual: [EMOCIÓN DEL DÍA]
- NO texto superpuesto
- Adecuada para profesionales de salud y público general
- Transmite información médica de manera tranquilizadora y positiva
- Incluye elementos orgánicos sutiles que sugieran salud y bienestar
```

## ElevenLabs — Audio

Cada artículo publicado genera automáticamente una versión en audio usando ElevenLabs con el modelo eleven_multilingual_v2 para español natural.

```json
{
  "model_id": "eleven_multilingual_v2",
  "voice_settings": {
    "stability": 0.75,
    "similarity_boost": 0.75,
    "style": 0.5,
    "use_speaker_boost": true
  }
}
```

-----

# 16. FRONTEND: DISEÑO Y UX

## Principios de Diseño

1. Minimalista — Sin anuncios, sin distracciones
1. Artístico — El contenido se presenta como arte, no como noticias genéricas
1. Accesible — WCAG 2.1 AA compliance mínimo
1. Responsivo — Mobile-first design
1. Rápido — Core Web Vitals óptimos gracias a Next.js SSR/SSG

## Paleta de Colores por Día

```css
:root {
  --monday: #87CEEB;    /* Azul Celeste */
  --tuesday: #FFD700;   /* Amarillo */
  --wednesday: #00CC00;  /* Verde */
  --thursday: #FF8C00;   /* Naranja */
  --friday: #FF0000;     /* Rojo */
  --saturday: #800080;   /* Morado */
  --sunday: #FFFFFF;     /* Blanco */
  --primary: #1a1a2e;    /* Dark background */
  --accent: #FF6B35;     /* Orange accent */
  --text: #EEEEEE;       /* Light text */
}
```

## Páginas Principales

| Ruta | Página | Descripción |
|------|--------|-------------|
| `/` | Home | Artículos destacados del día con color del día |
| `/articulos` | Feed de artículos | Grid filtrable por categoría/día/fecha |
| `/articulo/[slug]` | Detalle de artículo | Artículo completo con audio player |
| `/categorias` | Categorías | Vista de las 5 categorías |
| `/categoria/[slug]` | Artículos por categoría | Feed filtrado |
| `/nuestrasfuentes` | Fuentes | Todas las fuentes por continente |
| `/transparencia` | Transparencia | Política de transparencia |
| `/buscar` | Búsqueda | Búsqueda avanzada con Elasticsearch |
| `/perfil` | Perfil de usuario | Favoritos, historial, preferencias |
| `/sobre-nosotros` | About | Misión, visión, equipo |

## Componentes Clave

- **ArticleCard** — Card de artículo con cover art, título, resumen, audio toggle
- **DailyHeader** — Banner dinámico con color y temática del día
- **AudioPlayer** — Player persistente para escuchar artículos
- **SourceBadge** — Badge que muestra la fuente con link a transparencia
- **CategoryFilter** — Filtro visual por las 5 categorías
- **SearchBar** — Búsqueda con autocompletado semántico
- **FlowerOfTheDay** — Indicador visual de la flor del día
- **ChatBot** — Asistente interactivo flotante

-----

# 17. SEO Y METADATA

## Estrategia SEO

### On-Page

- Meta descriptions optimizadas (150-160 chars) por artículo
- Structured data (Schema.org) para artículos médicos
- URLs amigables: /articulo/titulo-del-articulo
- Sitemap XML generado automáticamente por Next.js
- Open Graph y Twitter Cards para compartir en redes
- Canonical URLs para evitar contenido duplicado
- Alt text en todas las imágenes

### Técnico

- SSR/SSG con Next.js para crawlability perfecta
- Core Web Vitals optimizados (LCP < 2.5s, FID < 100ms, CLS < 0.1)
- Lazy loading de imágenes y componentes
- robots.txt y meta robots configurados correctamente

### Contenido

- 3-5 artículos por semana consistentemente
- Keywords por categoría optimizados para intención de búsqueda médica
- Internal linking entre artículos relacionados
- Evergreen content marcado para re-promoción

-----

# 18. SISTEMA MULTI-AGENTE (MAS)

El proyecto implementa un sistema jerárquico estilo Crew.ai con agentes especializados.

## Agentes Disponibles

### 1. Project Manager (PM)
- Rol: Supervisión general del proyecto
- Meta: Coordinación, timelines, recursos, mitigación de riesgos
- Herramientas: Notion, ClickUp, n8n dashboards

### 2. Technical Architect (TA)
- Rol: Decisiones técnicas y arquitectura
- Meta: Sistemas escalables, integrados, mejores prácticas
- Herramientas: GitHub, Docker, Supabase, Vercel

### 3. UI/UX Specialist (UX)
- Rol: Diseño de interfaz y experiencia
- Meta: Diseños user-friendly, accesibles, atractivos
- Herramientas: Figma, Next.js, Tailwind

### 4. Content Curator (CC)
- Rol: Estrategia y curación de contenido
- Meta: Calidad, relevancia, SEO optimizado
- Herramientas: Strapi, OpenAI, fuentes médicas

### 5. AI Integration Expert (AI)
- Rol: Integración de IA y ML
- Meta: Chatbot, NLP, generación de contenido por IA
- Herramientas: OpenAI API, ElevenLabs, n8n

### 6. Data Scientist (DS)
- Rol: Modelado y análisis de datos
- Meta: Insights de comportamiento, personalización
- Herramientas: Supabase, Neo4j, Analytics

### 7. Security Specialist (SS)
- Rol: Privacidad y seguridad
- Meta: Compliance GDPR, auditorías, protección de datos
- Herramientas: Supabase RLS, RBAC

### 8. Performance Optimizer (PO)
- Rol: Rendimiento y optimización
- Meta: Velocidad, caching, eficiencia
- Herramientas: Vercel Analytics, Sentry, Lighthouse

## Modelo Jerárquico

```
NIVEL EJECUTIVO
├── Chief Operations Agent (COA) — Supervisión, KPIs, presupuesto
└── Chief Technology Agent (CTA) — Infraestructura, IA, escalabilidad

NIVEL GERENCIAL
├── Full-Stack Dev Manager (FSMA) — Equipo de desarrollo
├── Marketing Manager (MMA) — Estrategia de marketing
└── Content Manager (CMA) — Curación y calidad editorial

NIVEL OPERATIVO
├── Development Agents — Frontend, backend, AI integration
├── Marketing Agents — SEO, social media, ads
├── Content Agents — Redacción, edición, curación
└── Support Agents — Soporte técnico, usuarios
```

-----

# 19. PLAN DE MARKETING

## Análisis FODA

| | Positivo | Negativo |
|---|----------|----------|
| **Interno** | **Fortalezas:** Contenido curado y positivo, sin anuncios, accesibilidad gratuita, fuentes de alta calidad, formato visualmente atractivo | **Debilidades:** Dependencia de fuentes externas, recursos limitados para contenido original, necesidad de actualización tecnológica constante |
| **Externo** | **Oportunidades:** Demanda creciente de noticias veraces, expansión en mercados hispanohablantes, integración de nuevas tecnologías IA, contenido audiovisual | **Amenazas:** Competencia con medios tradicionales y digitales, cambios en algoritmos de distribución, desafíos de monetización a largo plazo |

## Estrategia de Canales

1. SEO Orgánico — Posicionamiento en Google para keywords médicas en español
1. Redes Sociales — X (Twitter), Instagram, LinkedIn, Facebook
1. Email Marketing — Newsletter semanal vía GoHighLevel
1. Programa de Referidos — Incentivos para usuarios que recomienden
1. Influencer Partnerships — Colaboraciones con médicos influencers
1. Content Marketing — Blog + artículos de alta calidad como herramienta de adquisición

## KPIs de Marketing

- Usuarios Activos Mensuales (MAU)
- Tasa de Crecimiento de Suscriptores
- Engagement (Tiempo en Plataforma, Artículos Leídos, Interacciones)
- Tasa de Producción de Contenido
- Customer Satisfaction Score (CSAT)

-----

# 20. PLAN FINANCIERO

## Objetivos Financieros

| Año | Revenue | Net Profit |
|-----|---------|------------|
| **Año 1** | $500,000 | $100,000 |
| **Año 3** | $5,000,000 | $1,500,000 |
| **Año 5** | $15,000,000 | $5,000,000 |

## Asignación de Presupuesto (Año 1: $500K)

| Categoría | % | Monto |
|-----------|---|-------|
| Desarrollo Tecnológico y AI | 40% | $200,000 |
| Curación y Optimización de Contenido | 30% | $150,000 |
| Marketing y Adquisición de Usuarios | 20% | $100,000 |
| Gastos Operativos | 10% | $50,000 |

## Revenue Streams

1. Premium Subscriptions — Contenido exclusivo, sin limits
1. Institutional Licenses — Hospitales, universidades, clínicas
1. Sponsored Content — Contenido patrocinado (claramente marcado)
1. Data Analytics Services — Insights para healthcare providers (futuro)
1. Virtual Events/Webinars — Eventos con expertos médicos (Año 3+)
1. Enterprise API — Acceso a datos curados para terceros (Año 3+)

-----

# 21. ROADMAP DE DESARROLLO POR FASES

## Fase 1: MVP Launch (Meses 1-6)

### Mes 1-2: Fundamentos

- [ ] Configurar Supabase: proyecto, tablas, auth, RLS
- [ ] Setup Next.js + Tailwind CSS + shadcn/ui
- [ ] Crear esquema de base de datos completo
- [ ] Configurar Docker + n8n
- [ ] Setup repositorio GitHub con CI/CD a Vercel
- [ ] Diseñar wireframes y mockups en Figma

### Mes 3-4: Core Development

- [ ] Desarrollar frontend: Home, ArticleDetail, Categories, Search
- [ ] Integrar Supabase auth y data fetching
- [ ] Configurar Strapi CMS headless
- [ ] Primer workflow n8n: Content sync Supabase → Notion
- [ ] Integrar OpenAI API para generación de contenido
- [ ] Implementar sistema de colores por día

### Mes 5: Integraciones

- [ ] Integrar ElevenLabs para audio de artículos
- [ ] Integrar DALL-E 3 para cover art con sistema floral
- [ ] Workflow n8n: Social distribution a X/Twitter
- [ ] Configurar GoHighLevel para newsletter
- [ ] Implementar búsqueda básica con Supabase full-text search

### Mes 6: Testing y Launch

- [ ] QA completo: unit tests, integration tests, UAT
- [ ] Cargar contenido inicial: 30-50 artículos
- [ ] Optimización de performance (Core Web Vitals)
- [ ] SEO setup: sitemap, robots, structured data
- [ ] Beta launch con grupo selecto de usuarios
- [ ] Iteración basada en feedback

## Fase 2: Growth (Meses 7-12)

- [ ] Mobile app (React Native)
- [ ] Chatbot interactivo con Dialogflow/Rasa
- [ ] Elasticsearch para búsqueda avanzada
- [ ] Programa de referidos
- [ ] Partnerships con influencers médicos
- [ ] Sistema de suscripción premium

## Fase 3: AI Enhancement (Año 2)

- [ ] Contenido en inglés
- [ ] Neo4j AuraDB para relaciones complejas (GraphRAG)
- [ ] Vector database para búsqueda semántica
- [ ] Personalización avanzada por usuario
- [ ] Data analytics dashboard

## Fase 4: Scale (Años 3-5)

- [ ] Diversificación de contenido (video, podcasts)
- [ ] Virtual events y webinars
- [ ] Enterprise API y soluciones B2B
- [ ] Expansión a más idiomas

-----

# 22. ASIGNACIÓN DE ROLES PARA LOS 5 AGENTES

## Distribución Recomendada

### AGENTE 1: Full-Stack Developer (Lead)

**Responsabilidad principal:** Frontend + Backend core

**Tareas:**
- Setup y mantenimiento de Next.js + Tailwind + shadcn/ui
- Integración con Supabase (auth, queries, real-time)
- Desarrollo de todas las páginas y componentes
- API layer (GraphQL/REST)
- Deployment en Vercel con CI/CD
- Performance optimization

**Stack que debe dominar:** React, Next.js, TypeScript, Tailwind CSS, Supabase, GraphQL

-----

### AGENTE 2: Backend & Database Engineer

**Responsabilidad principal:** Infraestructura de datos + Seguridad

**Tareas:**
- Diseño e implementación del esquema de Supabase (PostgreSQL)
- Configuración de RLS, RBAC, políticas de seguridad
- Setup y configuración de Strapi CMS
- Docker configuration para todos los servicios
- Configuración de Elasticsearch (Fase 2)
- Neo4j AuraDB setup (Fase 3)
- Backups, monitoreo, escalabilidad

**Stack que debe dominar:** PostgreSQL, Supabase, Docker, Strapi, Node.js, SQL

-----

### AGENTE 3: Automation & AI Engineer

**Responsabilidad principal:** n8n workflows + Integraciones de IA

**Tareas:**
- Setup y configuración de n8n (Docker)
- Desarrollo de TODOS los workflows automatizados (6+ workflows)
- Integración con OpenAI API (generación de contenido)
- Integración con DALL-E 3 (cover art)
- Integración con ElevenLabs (audio)
- Integración con GoHighLevel, Notion, Google Drive, Airtable
- Social media automation (X/Twitter API)
- Chatbot development (Fase 2)

**Stack que debe dominar:** n8n, REST APIs, OpenAI API, Docker, Node.js, JSON

-----

### AGENTE 4: Content Curator & SEO Specialist

**Responsabilidad principal:** Contenido editorial + SEO + Marketing

**Tareas:**
- Curación diaria de contenido de las 19+ fuentes internacionales
- Revisión y edición de artículos generados por IA
- Implementación del sistema de personalidad semanal
- Aplicación del sistema floral mensual
- SEO on-page: meta descriptions, keywords, structured data
- Estrategia de contenido y calendario editorial
- Gestión de redes sociales y newsletter
- Tracking de KPIs de marketing

**Skills que debe dominar:** Escritura médica, SEO, español impecable, marketing digital, Strapi CMS

-----

### AGENTE 5: UI/UX Designer & QA

**Responsabilidad principal:** Diseño visual + Testing + Quality Assurance

**Tareas:**
- Diseño de todas las interfaces en Figma
- Implementación de la paleta de colores por día
- Design system con componentes reutilizables
- Sistema visual floral para cover art
- Responsive design testing (mobile-first)
- WCAG 2.1 AA accessibility compliance
- QA: unit testing, integration testing, UAT
- Bug tracking y regression testing
- Documentation de componentes

**Skills que debe dominar:** Figma, UI/UX design, Tailwind CSS, testing frameworks, accesibilidad

-----

# 23. RIESGOS Y MITIGACIÓN

| Riesgo | Impacto | Probabilidad | Estrategia de Mitigación |
|--------|---------|--------------|--------------------------|
| Baja adopción de usuarios | Alto | Medio | Marketing agresivo, engagement comunitario, feedback constante |
| Problemas técnicos | Alto | Bajo | QA riguroso, equipo de soporte responsivo, monitoring |
| Compromiso de calidad de contenido | Alto | Bajo | Curadores calificados, guidelines editoriales estrictas, human-in-the-loop |
| Fallas en algoritmos de IA | Medio | Medio | Entrenamiento continuo, feedback integration, supervisión humana |
| No-compliance regulatorio | Alto | Bajo | Expertise legal, auditorías regulares de compliance |
| Competencia de mercado | Medio | Alto | Propuesta de valor única, innovación continua |
| Shortfalls financieros | Alto | Medio | Fuentes diversas de funding, reservas financieras |

-----

# 24. CHECKLIST DE LANZAMIENTO MVP

## Pre-Launch (2 semanas antes)

- [ ] Todos los servicios configurados y funcionando (Supabase, Strapi, n8n, Vercel)
- [ ] Mínimo 30 artículos publicados cubriendo las 5 categorías
- [ ] Audio generado para al menos 10 artículos
- [ ] Cover art generado para todos los artículos
- [ ] Sistema de colores por día funcionando correctamente
- [ ] Auth flow completo (registro, login, perfil)
- [ ] Búsqueda funcionando
- [ ] Mobile responsive verificado en 3+ dispositivos
- [ ] SEO basics: sitemap, robots.txt, meta tags, Open Graph
- [ ] SSL certificado activo
- [ ] Google Analytics / Sentry configurados
- [ ] Pruebas de carga realizadas
- [ ] Backup automático configurado en Supabase

## Launch Day

- [ ] DNS apuntando correctamente a Vercel
- [ ] n8n workflows activados (content sync, social distribution)
- [ ] Newsletter de lanzamiento preparada en GoHighLevel
- [ ] Posts de lanzamiento programados en X/Twitter
- [ ] Equipo en stand-by para monitorear y resolver issues
- [ ] Notificar a beta testers del launch público

## Post-Launch (primeras 2 semanas)

- [ ] Monitorear métricas diariamente (traffic, engagement, errors)
- [ ] Responder feedback de usuarios dentro de 24 horas
- [ ] Publicar mínimo 3 artículos por semana
- [ ] Revisar y optimizar workflows de n8n
- [ ] Primera retrospectiva de equipo
- [ ] Ajustar prioridades basado en datos reales

-----

# 25. APÉNDICES Y REFERENCIAS TÉCNICAS

## A. Notion Databases Necesarias

1. Content Tracker — Title, Summary, Category, Status, Publication Date, Author
1. Project Management — Project Name, Status, Deadlines, Assigned Team Members
1. Feedback Management — Feedback ID, Article ID, User ID, Comment, Rating, Date

## B. API Keys Necesarias (obtener antes de empezar)

1. Supabase (URL + Anon Key + Service Role Key)
1. OpenAI (API Key)
1. ElevenLabs (API Key)
1. Notion (Internal Integration Token)
1. X/Twitter (API Key, Secret, Access Token)
1. GoHighLevel (API Key)
1. Google (Analytics ID, Drive API credentials)
1. Vercel (Account + Team setup)
1. GitHub (Organization + repo setup)

## C. Docker Services

```yaml
version: '3'
services:
  n8n:
    image: n8nio/n8n
    ports: ["5678:5678"]
    volumes: [n8n_data:/root/.n8n]
  strapi:
    image: strapi/strapi
    ports: ["1337:1337"]
    volumes: [strapi_data:/srv/app]
    depends_on: [supabase]
  frontend:
    build: ./frontend
    ports: ["3000:3000"]

volumes:
  n8n_data:
  strapi_data:
```

## D. Modelo de GraphRAG (Neo4j) — Fase 3

```
Nodos: Article, Author, Category, Tag, Theme, Source, Edition

Relaciones:
(Article)-[:WRITTEN_BY]->(Author)
(Article)-[:BELONGS_TO]->(Category)
(Article)-[:TAGGED_WITH]->(Tag)
(Article)-[:COVERS_THEME]->(Theme)
(Article)-[:SOURCED_FROM]->(Source)
(Author)-[:SPECIALIZES_IN]->(Theme)
(Theme)-[:RELATED_TO]->(Theme)
```

## E. Contactos Clave

- Dominio: www.medicanoticia.com
- Hosting: Vercel
- Database: Supabase
- CMS: Strapi
- Automation: n8n
- CRM: GoHighLevel

-----

## NOTA FINAL PARA EL EQUIPO

Este documento contiene todo lo necesario para construir Medica Noticia desde cero. Cada sección está diseñada para ser actionable — no es teoría, es un plan de ejecución.

**Prioridades inmediatas:**

1. Agente 2: Setup Supabase + Docker + esquema de DB
1. Agente 1: Setup Next.js + Tailwind + Vercel + Supabase client
1. Agente 5: Wireframes en Figma + Design system
1. Agente 3: Setup n8n + primer workflow (content sync)
1. Agente 4: Curar primeros 30 artículos + setup calendario editorial

El objetivo es tener un MVP funcional en 6 meses. Cada sprint de 2 semanas debe producir incrementos demostrables.

¡Vamos a construir la principal fuente de información médica en español! 🚀

-----

*Documento generado a partir del Knowledge Base completo del proyecto Medica Noticia.*
*Versión 1.0 — Febrero 2026*
