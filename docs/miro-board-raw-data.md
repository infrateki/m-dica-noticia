# Médica Noticia — Miro Board Raw Data

*Complete text extraction from Miro board — February 8, 2026*

---

## GALENUS Database Schema (Supabase + Neo4j)

### Entity Relationships
```
USUARIO ||--o{ SUSCRIPCION : tiene
USUARIO ||--o{ COMENTARIO : escribe
USUARIO ||--o{ FAVORITO : guarda
USUARIO ||--o{ HISTORIAL_LECTURA : registra
ARTICULO ||--o{ COMENTARIO : recibe
ARTICULO ||--o{ FAVORITO : es_marcado
ARTICULO ||--o{ HISTORIAL_LECTURA : es_leido
PUBLICACION ||--o{ ARTICULO : contiene
CATEGORIA ||--o{ ARTICULO : clasifica
AUTOR ||--o{ ARTICULO : escribe
CLIENTE ||--o{ ANUNCIO : publica
ANUNCIO ||--o{ PUBLICACION : aparece_en
USUARIO ||--o{ NOTIFICACION : recibe
```

### Tables

- **USUARIO** — id, email, nombre_completo, hashed_password, created_at, last_login, is_active, rol
- **SUSCRIPCION** — id, usuario_id, tipo, fecha_inicio, fecha_fin, auto_renovacion, estado
- **COMENTARIO** — id, usuario_id, articulo_id, contenido, created_at, is_approved
- **FAVORITO** — id, usuario_id, articulo_id, created_at
- **HISTORIAL_LECTURA** — id, usuario_id, articulo_id, fecha_lectura, tiempo_lectura
- **ARTICULO** — id, publicacion_id, categoria_id, titulo, resumen, contenido, fecha_publicacion, autor_ids[], palabras_clave[], estado
- **PUBLICACION** — id, titulo, fecha_publicacion, numero_edicion, tipo
- **CATEGORIA** — id, nombre, descripcion
- **AUTOR** — id, nombre, apellido, email, biografia, especialidades[]
- **CLIENTE** — id, nombre, contacto_email, telefono, fecha_inicio_relacion
- **ANUNCIO** — id, cliente_id, titulo, descripcion, fecha_inicio, fecha_fin, tipo, estado
- **NOTIFICACION** — id, usuario_id, tipo, contenido, created_at, is_read

---

## Floral System — Additional Details

### Octubre
- **Caléndula** (Marigold)
- Arte inspiración: https://www.reprodart.com/a/abstrahiertfigurativeku.html

### Septiembre
- **Flor Lirio de Jengibre** (Ginger Lily)
- Sep 1-30: Mes de la Concienciación sobre el Cáncer Infantil (EE.UU.)
- 21 de Septiembre: Día Mundial del Alzheimer
  - Artículo: "Innovaciones en el Tratamiento del Alzheimer: Nuevas Esperanzas"
- 29 de Septiembre: Día Mundial del Corazón
  - Artículo: "Cuidando el Corazón: Avances en la Salud Cardiovascular"

### Noviembre
- **Crisantemo** (Chrysanthemum)
- **Poinsettia**

### Diciembre
- **Crisantemo** / **Poinsettia**

---

## Social Media Strategy (from Miro)

### Pinterest Strategy
- **Promoción de Contenido:**
  - Aumento de Visibilidad: Publicar imágenes o infografías atractivas con enlaces al sitio
  - Uso de Rich Pins: Mostrar información adicional directamente en el pin
- **Construcción de Comunidad:**
  - Interacción con cuentas de salud, comentar en pines relevantes
  - Educación Visual: Infografías sobre temas médicos
- **Monetización y Colaboraciones:**
  - Colaboraciones con marcas de salud y bienestar
  - Ventas de productos digitales (e-books, cursos)

### YouTube Strategy
- Videos educativos: crear contenido del artículo en formato video
- Los videos se pueden hacer shorts y publicarlos en las demás redes
- Eventualmente postear videos regularmente

### Content Calendar Structure
- **Semana 1-4** rotation per month
- Each week has assigned articles by day
- "Personalidad del mes" — monthly theme personality

---

## Article Examples (from Miro)

- "Mapeo Cerebral: Revolucionando la Comunicación para Personas con Parálisis" (19 Agosto)
- "Interfaces Cerebro-Computadora mapean la corteza prefrontal, descifrando el lenguaje del pensamiento. Estudio en pacientes con epilepsia abre puertas a la comunicación en parálisis severa."
- "Descubren cura contra el cancer" (example headline)
- "Innovaciones en el Tratamiento del Alzheimer: Nuevas Esperanzas"
- "Cuidando el Corazón: Avances en la Salud Cardiovascular"

---

## Visual Inspiration

- **Stanford Medicine Magazine** — primary layout inspiration ("Stanford style")
- **Photographer:** Ornan Rodriguez (https://www.pexels.com/es-es/@ornanvelazquez/)
- **MidJourney art:** https://cdn.midjourney.com/596825d9-bc13-45b7-8766-be8eb33b2789/0_3.png
- **Art reference:** https://www.reprodart.com/a/abstrahiertfigurativeku.html

---

## Operational Notes

### Weekly Agenda
- Revisión de la Web: Lunes, Jueves, Domingo
- Revisión de Fuentes: Martes, Viernes
- Creación de Contenido: Lunes, Miércoles, Viernes, Domingo
- Creación de Arte: Martes, Jueves, Sábado
- Reuniones de Equipo: Lunes, Martes, Jueves
- Actualización de Redes Sociales: Miércoles, Viernes, Domingo

### Content Flow per Day
Each day shows: últimas noticias, descubrimientos, salud, innovación, tecnología, mundo
With article slots: articulo 1-4, redes sociales post, enlaces + keywords

---

*Raw data extracted from Miro board by Dani — February 8, 2026*
*Original work by Sergio Villanueva Meyer & Daniela (~2024)*
