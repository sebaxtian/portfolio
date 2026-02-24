# Portfolio Website - Sebastián Ríos Sabogal

A professional, high-conversion portfolio website for Sebastián Ríos Sabogal, a Data Engineer and DevOps Specialist.

![Portfolio Preview](assets/images/og-image.jpg)

## 🚀 Features

- **Modern Dark Theme** - Professional design with teal accents
- **Fully Responsive** - Optimized for all devices (mobile, tablet, desktop)
- **SEO Optimized** - Meta tags, Open Graph, and structured data
- **High Performance** - Lazy loading, optimized assets
- **Accessible** - WCAG 2.1 AA compliant
- **Interactive** - Smooth animations and transitions

## 📁 Project Structure

```
portfolio/
├── index.html              # Main HTML file
├── css/
│   └── styles.css          # Custom CSS styles and animations
├── js/
│   └── main.js             # JavaScript interactions
├── assets/
│   ├── images/
│   │   └── favicon.svg     # Site favicon
│   └── documents/
│       └── cv-sebastianrioss-esp.pdf
├── plans/
│   └── portfolio-website-plan.md  # Detailed planning document
└── README.md
```

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first CSS framework (via CDN)
- **Vanilla JavaScript** - No framework dependencies
- **Google Fonts** - Inter & JetBrains Mono

## 📋 Sections

### 1. Hero Section
- Impact headline with value proposition
- Dual CTAs (View Projects / Contact)
- Tech stack icons
- Animated background

### 2. Sobre Mí (About Me)
- Professional narrative
- Key statistics (10+ years, 20+ technologies, 15+ projects)
- Technical skills tags
- Career timeline

### 3. Servicios (Services)
- Data Engineering
- DevOps & Cloud
- Full-Stack Development
- Web Scraping
- GIS Solutions
- Technical Consulting

### 4. Portafolio (Portfolio)
Featured projects:
- **Tangara** - Air Quality Monitoring Network
- **Electoral Monitoring** - International election data collection
- **SIRA** - Academic Registration System
- **Leonardo247** - Property Management System
- **MAPFRE Data Lake** - Business Intelligence
- **GisData** - Geographic Information System

### 5. Contacto (Contact)
- Direct contact information
- Professional profile links
- Contact form (mailto)

## 🎨 Color Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Background Primary | `#0f172a` | Main background |
| Background Secondary | `#1e293b` | Cards, sections |
| Accent Primary | `#14b8a6` | Teal - CTAs, highlights |
| Accent Secondary | `#06b6d4` | Cyan - Gradients |
| Text Primary | `#f8fafc` | Headings |
| Text Secondary | `#cbd5e1` | Body text |

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

## 📱 Responsive Breakpoints

| Breakpoint | Width | Target |
|------------|-------|--------|
| `sm` | 640px | Small phones |
| `md` | 768px | Tablets |
| `lg` | 1024px | Laptops |
| `xl` | 1280px | Desktops |
| `2xl` | 1536px | Large screens |

## ⚡ Performance Optimizations

- **Tailwind CSS via CDN** - Only loads used styles
- **Lazy Loading** - Images load on scroll
- **Minimal JavaScript** - No heavy frameworks
- **Optimized Fonts** - Preconnect to Google Fonts
- **SVG Favicon** - Small file size, scalable

## 🔍 SEO Features

- Semantic HTML5 structure
- Meta description and keywords
- Open Graph tags for social sharing
- Twitter Card support
- JSON-LD structured data
- Proper heading hierarchy
- Alt text ready for images

## 📧 Contact Form

The contact form uses the `mailto:` protocol, which opens the user's default email client. For a production site, consider integrating:

- [Formspree](https://formspree.io/)
- [Netlify Forms](https://www.netlify.com/products/forms/)
- [Google Forms](https://forms.google.com/)
- Custom backend API

## 🔧 Customization

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

## 📄 License

This project is created for Sebastián Ríos Sabogal. Feel free to use the structure and design as inspiration for your own portfolio.

## 🤝 Contact

**Sebastián Ríos Sabogal**
- Email: sebaxtianrioss@gmail.com
- LinkedIn: [sebastianriossabogal](https://www.linkedin.com/in/sebastianriossabogal/)
- About.me: [sebaxtian](https://about.me/sebaxtian)
- Blog: [ideafalaz.blogspot.com](https://ideafalaz.blogspot.com)

---

*Built with ❤️ using HTML5, Tailwind CSS, and Vanilla JavaScript*
