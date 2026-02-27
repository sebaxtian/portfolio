# Portfolio Website - Sebastian Rios Sabogal

A professional, high-conversion portfolio website showcasing the expertise of **Sebastian Rios Sabogal**, a Data Engineer, DevOps & Full-Stack Specialist. This project serves as a digital gateway to his technical trajectory, combining corporate excellence with social impact.

<div align="center">
  <img src="assets/images/og-image.png" alt="Portfolio Preview" width="100%">
  <br>
  <h3>Data Engineering | DevOps | Full-Stack Development</h3>
  <p><i>"Transforming data into high-impact strategic solutions."</i></p>
  
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Sebastian_Rios-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/sebastianriossabogal/)
  [![GitHub](https://img.shields.io/badge/GitHub-sebaxtian-1e293b?style=flat-square&logo=github)](https://github.com/sebaxtian/)
  [![Website](https://img.shields.io/badge/Website-sebaxtian.dev-teal?style=flat-square)](https://sebaxtian.dev/)
</div>

---

## 🚀 Key Features

- **Modern Dark Theme** - Professional design with teal accents
- **Fully Responsive** - Optimized for all devices (mobile, tablet, desktop)
- **SEO Optimized** - Meta tags, Open Graph, and structured data
- **High Performance** - Lazy loading, optimized assets
- **Accessible** - WCAG 2.1 AA compliant
- **Interactive** - Smooth animations and transitions

---

## 📁 Project Structure

```bash
portfolio/                  # Root directory
├── index.html              # Main production HTML file
├── css/                    # Custom CSS styles and animations
│   └── styles.css
├── js/                     # JavaScript interactions
│   └── main.js
├── assets/                 # Asset folder
│   ├── images/             # Branding assets and favicons
│   └── documents/          # Placeholder for documents (CV, etc.)
├── templates/              # Versioned evolution of the design (v1, v2, v3)
├── plans/                  # Strategic roadmaps and project planning
└── README.md               # This documentation
```

---

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first CSS framework (via CDN)
- **Vanilla JavaScript** - No framework dependencies
- **Google Fonts** - Inter & JetBrains Mono

---

## 📋 Sections

### 1. Hero Section
- Impact headline with value proposition
- Dual CTAs (View Trayectoria / GitHub Profile)
- Tech stack icons (Python, AWS, Docker, PostgreSQL, PySpark, FastAPI, Linux, Pandas)
- Animated background and scroll indicator

### 2. Propuesta de Valor (Value Proposition)
- Intersection of corporate excellence and social impact
- Key statistics (+10 years, +340k data processed, +20 technologies, +15 projects)
- Focus on GIS and Open Source

### 3. Servicios (Services)
- Cloud & DevOps (AWS, Terraform, Docker)
- Data Engineering (PySpark, dbt, Snowflake)
- Development & GIS (FastAPI, PostGIS, Angular)
- Automatización Low-Code (n8n, Zapier, Make)
- Machine Learning & Data Science (Scikit-learn, Polars, Pandas)
- Scrum & Agile Development (Scrum, Kanban, Lean)

### 4. Trayectoria Profesional (Professional Experience)
- **Solidaridad Colombia** - Data Engineer & DevOps (2024 - Present)
- **F. Herencia Cultural Guatemalteca** - Web Scraping Developer (2024)
- **NetMidas & Aliados** - Backend & Data Engineer (2019 - 2023)
- **GeoProcess S.A.S.** - GIS Specialist & Full-Stack Developer (2014 - 2019)

### 5. Educación e Innovación (Education & Innovation)
- Formación Base (Ingeniería de Sistemas, Tecnología en Sistemas de Información)
- Diplomados (Arquitectura de Software, Machine Learning, Big Data)
- Cursos y Certificaciones (n8n, AI, AWS, Snowflake, Scrum)

### 6. Portafolio (Portfolio)
Featured projects:
- **Tangara** - Air Quality Monitoring Network
- **Electoral Monitoring** - International election data collection
- **SIRA** - Academic Registration System
- **Datapico** - Data Journalism Pipeline/ETL as Marketing
- **Leonardo247** - Property Management System
- **MAPFRE Data Warehouse** - Data Warehouse and Business Intelligence
- **GisData** - Geographic Information System

### 7. Contacto (Contact)
- Direct contact information
- Professional profile links (LinkedIn, GitHub, Blog)

---

## 📄 Templates

The project maintains versioned templates to track the evolution of the design and structure:

- **v1**: Initial layout and basic structure.
- **v2**: Refined design with improved responsiveness.
- **v3**: Current production-ready template with full feature set.

---

## 🎨 UI/UX Design Decisions

The project's visual identity is defined by a **Deep Slate & Teal** theme, extracted from the core branding:

- **Primary Background:** `#0f172a` (Slate 900) for a focused, professional environment.
- **Accent Color:** `#14b8a6` (Teal 500) representing precision and innovation.
- **Typography:** A dual-font system balancing human-centric readability with technical rigor.
- **Animations:** Subtle fade-ins and staggered delays to guide the user's attention through the professional narrative.

### 🎨 Color Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Background Primary | `#0f172a` | Main background |
| Background Secondary | `#1e293b` | Cards, sections |
| Accent Primary | `#14b8a6` | Teal - CTAs, highlights |
| Accent Secondary | `#06b6d4` | Cyan - Gradients |
| Text Primary | `#f8fafc` | Headings |
| Text Secondary | `#cbd5e1` | Body text |


### 📱 Responsive Breakpoints

| Breakpoint | Width | Target |
|------------|-------|--------|
| `sm` | 640px | Small phones |
| `md` | 768px | Tablets |
| `lg` | 1024px | Laptops |
| `xl` | 1280px | Desktops |
| `2xl` | 1536px | Large screens |

### ⚡ Performance Optimizations

- **Tailwind CSS via CDN** - Only loads used styles
- **Lazy Loading** - Images load on scroll
- **Minimal JavaScript** - No heavy frameworks
- **Optimized Fonts** - Preconnect to Google Fonts
- **SVG Favicon** - Small file size, scalable

---

## 🔍 SEO Features

- Semantic HTML5 structure
- Meta description and keywords
- Open Graph tags for social sharing
- Twitter Card support
- JSON-LD structured data
- Proper heading hierarchy
- Alt text ready for images

---

## 🔧 Customization

- **Branding:** Update the `tailwind.config` object in `index.html` to modify the color scheme.
- **Content:** Project cards and professional experience are managed directly in the semantic HTML structure.
- **SEO:** Meta tags and structured data are located in the `<head>` section for easy indexing optimization.

### Changing Colors

Edit the Tailwind config in `index.html`:

```javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                // Add custom colors here
            }
        }
    }
}
```

### Adding Projects

Copy a project card in the Portfolio section and update:
- Title
- Description
- Technologies
- Links
- Status badge

### Adding Profile Photo

1. Add your photo to `assets/images/`
2. Update the About section with an `<img>` tag
3. Recommended size: 400x400px

---

## 🚀 Getting Started

### Local Development

1. Clone or download the repository
2. Open `index.html` in your browser
3. No build process required!

### Using a Local Server (Optional)

```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

---

## 📬 Contact & Collaboration

Sebaxtian is always open to new technical challenges and impact-driven collaborations.

- **LinkedIn:** [sebastianriossabogal](https://www.linkedin.com/in/sebastianriossabogal/)
- **Blog:** [ideafalaz.blogspot.com](https://ideafalaz.blogspot.com/)
- **Email:** sebaxtianrioss@gmail.com
- **Website:** [sebaxtian.dev](https://sebaxtian.dev/)

---

## 📄 License

This project is created for Sebastian Rios Sabogal. Feel free to use the structure and design as inspiration for your own portfolio.

---
<p align="center"><i>Built with ❤️ using HTML5, Tailwind CSS, and Vanilla JavaScript</i></p>
