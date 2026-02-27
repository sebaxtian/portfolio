# Technical Plan: index-v1.html Merge

This plan outlines the strategy for merging the visual style of [`index.html`](index.html) with the content and structure of [`index-gemini.html`](index-gemini.html).

## 1. Visual Identity (from index.html)
- **Color Palette:**
  - Background: `bg-slate-900` (#0f172a)
  - Primary Accent: `teal-400` (#2dd4bf) / `teal-500`
  - Secondary Accent: `cyan-400`
  - Text: `slate-100` (Primary), `slate-300` (Secondary), `slate-400` (Muted)
  - Borders: `slate-800/50`
- **Typography:**
  - Sans: 'Inter', system-ui, sans-serif
  - Mono: 'JetBrains Mono', monospace
- **UI Components:**
  - Glassmorphism effects (backdrop-blur-md)
  - Gradient text and buttons
  - Animated grid backgrounds
  - Custom scrollbar (slate-900 track, slate-300/teal-400 thumb)

## 2. Content & Structure (from index-gemini.html)
- **Sections to preserve:**
  - Navigation (with `<sebaxtian />` logo style)
  - Hero Section (Personalized greeting and specific CTA)
  - Propuesta de Valor (Value Proposition)
  - Áreas de Expertise (Services with specific badges like "Diplomado UNAL")
  - Trayectoria Profesional (Detailed experience timeline)
  - Educación e Innovación (Education, Diplomados, and Certifications)
  - Portafolio de Proyectos (Detailed project cards)
  - Contacto (Form and social links)

## 3. Technical Implementation
- **Framework:** Tailwind CSS (via CDN with custom config).
- **SEO:**
  - Use `<header>`, `<main>`, `<section>`, `<footer>`.
  - Proper `<h1>` to `<h3>` hierarchy.
  - Meta tags for Open Graph and Twitter (from index.html).
  - JSON-LD Structured Data (from index.html).
- **Performance:**
  - Optimized SVG icons.
  - Efficient Tailwind classes.
  - Minimal custom CSS.

## 4. Merge Strategy
1.  **Head Section:** Use the comprehensive meta tags and font imports from [`index.html`](index.html).
2.  **Tailwind Config:** Port the `slate-850` and font family definitions.
3.  **Body Classes:** Apply `bg-slate-900 text-slate-100 font-sans antialiased`.
4.  **Component Mapping:**
    - Replace `index-gemini.html`'s `.glass-card` with the border/background style from `index.html`.
    - Use the `teal-400` gradient buttons from `index.html` for all CTAs.
    - Apply the "Animated Grid Background" to the Hero section.
