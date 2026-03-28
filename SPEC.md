# Mattera Web - SPEC.md

## 1. Concept & Vision

Landing page para Mattera, empresa de automatizaciones para negocios. Tono profesional pero accesible, con estética tech oscura. Transmite confianza, innovación y eficiencia. El visitantes debe sentir que está ante expertos que simplifican su negocio.

## 2. Design Language

### Aesthetic Direction
Minimalismo tecnológico oscuro — inspirado en interfaces de SaaS modernas (Linear, Vercel). Espacios amplios, tipografía bold, acentos de color que guían la vista.

### Color Palette
- **Background**: `#0a0a0a` (negro profundo)
- **Surface**: `#141414` (cards/sections)
- **Border**: `#262626`
- **Text Primary**: `#ffffff`
- **Text Secondary**: `#a1a1a1`
- **Accent**: `#6366f1` (indigo vibrante)
- **Accent Hover**: `#818cf8`

### Typography
- **Headings**: Inter (700, 600) - sans-serif geométrica moderna
- **Body**: Inter (400, 500)
- **Fallback**: system-ui, sans-serif

### Spatial System
- Base unit: 8px
- Section padding: 80px-120px vertical
- Container max-width: 1200px
- Card border-radius: 16px
- Button border-radius: 8px

### Motion Philosophy
- Fade-in on scroll (opacity 0→1, translateY 20px→0, 600ms ease-out)
- Hover en cards: subtle lift (translateY -4px, shadow increase)
- Buttons: scale 1.02 + glow en hover
- Form inputs: border-color transition 200ms

### Visual Assets
- Logo Mattera en versión white (invertido del original)
- Iconos: Lucide icons (línea fina, estilo minimalista)
- Decorativos: gradientes sutiles, bordes con glow

## 3. Layout & Structure

### Hero Section
- Logo Mattera centered
- Headline impactante: "Automatiza tu negocio. Escala sin límites."
- Subheadline con propuesta de valor
- CTA principal: "Solicitar Cotización"
- Badge: "Más de 50 negocios automatizados en Jalisco"

### Servicios Section
- Grid 3 columnas (responsive a 2 y 1)
- Cards con icono, título y descripción breve
- Servicios:
  - Chatbots inteligentes
  - Agentes IA
  - CRM personalizado
  - Integraciones de sistemas
  - Automatización de procesos
  - Reportes y analytics

### Por Qué Mattera Section
- 3 features diferenciadoras
- Estadísticas (números grandes)
- Tono más emocional/personal

### Proceso Section
- 4 pasos del proceso de trabajo
- Timeline visual minimalista

### Contacto Section
- Formulario con campos:
  - Nombre completo
  - Email empresarial
  - Teléfono/WhatsApp
  - Nombre del negocio
  - Tipo de automatización (select)
  - Describe tu proyecto (textarea)
- Info de contacto directo
- Ubicación: Guadalajara, Jalisco

### Footer
- Logo pequeño
- Links rápidos
- Copyright

## 4. Features & Interactions

### Navigation
- Header sticky con blur backdrop
- Scroll suave a secciones
- Botón CTA siempre visible

### Contact Form
- Validación en tiempo real
- Estados: default, focus, error, success
- On submit: mensaje de confirmación (no requiere backend por ahora - solo UI)
- Campos requeridos con asterisco

### Scroll Animations
- Elementos aparecen con fade-in al entrar en viewport
- Stagger de 100ms entre elementos de mismo grupo

### Responsive
- Mobile-first
- Breakpoints: 640px, 768px, 1024px
- Nav mobile: menu hamburguesa

## 5. Component Inventory

### Button Primary
- BG: accent (#6366f1)
- Text: white
- Padding: 14px 28px
- Hover: accent-hover + subtle glow + scale 1.02
- Active: scale 0.98

### Button Secondary
- BG: transparent
- Border: 1px solid #262626
- Text: white
- Hover: border-color accent

### Card Service
- BG: surface (#141414)
- Border: 1px solid #262626
- Padding: 32px
- Icon: 48px, accent color
- Hover: border-color accent, lift

### Input Field
- BG: transparent
- Border: 1px solid #262626
- Padding: 14px 16px
- Focus: border-color accent
- Error: border-color red (#ef4444)

### Badge
- BG: accent con 10% opacity
- Text: accent
- Padding: 6px 12px
- Border-radius: 20px

## 6. Technical Approach

- **Stack**: HTML + CSS + Vanilla JS (single file por simplicity)
- **Fonts**: Google Fonts (Inter)
- **Icons**: Lucide CDN
- **Animations**: CSS + Intersection Observer API
- **Form**: Client-side validation, success state
- **Deploy**: GitHub Pages (mismo repo o nuevo)

## 7. Content

### Hero
- Headline: "Automatiza tu negocio. Escala sin límites."
- Sub: "En Mattera creamos soluciones de automatización personalizadas para negocios que quieren crecer eficientemente. Chatbots, CRMs, integraciones y más."

### Servicios
1. **Chatbots Inteligentes**: Atención a clientes 24/7 con IA que entiende y responde.
2. **Agentes IA**: Automatiza tareas repetitivas con agentes inteligentes.
3. **CRM Personalizado**: Gestiona tus clientes y ventas a tu manera.
4. **Integraciones**: Conecta todos tus sistemas y elimina el trabajo manual.
5. **Automatización de Procesos**: streamline flujos de trabajo empresariales.
6. **Reportes y Analytics**: Datos que te ayudan a tomar mejores decisiones.

### Por Qué Mattera
- **Rapidez**: Implementamos en semanas, no meses.
- **Personalización**: Soluciones a tu medida, no plantillas.
- **Soporte**: Accompañamiento continuo post-implementación.

### Stats
- 50+ Negocios automatizados
- 95% Satisfacción de clientes
- 3+ Años de experiencia

### Proceso
1. Diagnóstico - Escuchamos tu negocio y detectamos oportunidades
2. Propuesta - Diseñamos la solución perfecta para ti
3. Implementación - Desarrollamos y conectamos todo
4. Soporte - Te acompañamos y optimizamos constantemente

### Contact Form Options (Tipo de automatización)
- Chatbot
- Agente IA
- CRM
- Integración
- Automatización de procesos
- Otro
