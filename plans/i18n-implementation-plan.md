# Plan: Sistema de Internacionalización (i18n) Bilingüe

## 1. Análisis del Proyecto
Se ha analizado la estructura actual del sitio web:
- **Tipo**: Sitio web estático (HTML/CSS/JS).
- **Contenido Actual**:
  - `index.html`: Versión en Español (82,973 bytes).
  - `index.en.html`: Versión en Inglés (82,510 bytes).
- **Navegación**: Utiliza anclajes (`#inicio`, `#experiencia`, etc.) dentro de la misma página.

## 2. Arquitectura de la Solución
Se implementará una estructura de rutas estáticas para maximizar el SEO y la caché del navegador.

### Estructura de Archivos Propuesta
```text
/
├── index.html              # Redirección automática (detecta idioma o redirige a /es/)
├── en/
│   └── index.html          # Contenido Inglés (actual index.en.html)
├── es/
│   └── index.html          # Contenido Español (actual index.html)
├── assets/                 # Recursos compartidos (CSS, JS, Imágenes)
└── js/
    └── i18n.js             # Lógica de redirección e internacionalización
```

## 3. Plan de Implementación

### Fase 1: Reestructuración de Archivos
- [ ] Crear directorio `es/`.
- [ ] Mover `index.html` a `es/index.html`.
- [ ] Crear directorio `en/`.
- [ ] Mover `index.en.html` a `en/index.html`.
- [ ] Actualizar rutas de recursos (imágenes, CSS) en ambos archivos si es necesario (deberían funcionar con rutas relativas `../assets/` si están en subcarpetas, o mejor, usar absolutas `/assets/`). *Nota: El código actual usa rutas relativas como `assets/images/...`. Al mover a subcarpetas, debemos cambiarlas a absolutas `/assets/...` para que funcionen correctamente.*

### Fase 2: Lógica de Redirección (Root `index.html`)
- [ ] Crear `index.html` en la raíz.
- [ ] Implementar script simple:
    1. Verificar `localStorage` (preferencia guardada).
    2. Si no hay preferencia, verificar `navigator.language`.
    3. Redirigir a `/es/` o `/en/` según corresponda.

### Fase 3: Interfaz del Selector de Idioma
- [ ] Agregar componente "Language Switcher" en la barra de navegación (`<nav>`) de `es/index.html` y `en/index.html`.
- [ ] **Diseño**:
    - Botón/Sección en el header.
    - Iconos de banderas (🇪🇸 para Español, 🇬🇧 para Inglés).
    - Etiqueta de acceso visual (aria-label).
- [ ] **Lógica JS**:
    - Al hacer clic, guardar preferencia en `localStorage`.
    - Redirigir a la otra versión (ej. de `/es/` a `/en/`).
    - Mantener el ancla actual si es posible (ej. redirigir a `/en/#experiencia`).

### Fase 4: Optimización SEO
- [ ] Añadir etiquetas `<link rel="alternate" hreflang="..." />` en el `<head>` de ambas páginas.
- [ ] Asegurar meta descripciones únicas y correctas para cada idioma.

## 4. Especificaciones Técnicas

### Javascript (Lógica de Redirección)
```javascript
// Pseudocódigo para root index.html
const lang = localStorage.getItem('preferredLang') || navigator.language;
const targetLang = lang.startsWith('es') ? '/es/' : '/en/';
window.location.href = targetLang;
```

### CSS (Selector de Idioma)
- Estilo visual: Botón minimalista con banderas.
- Posición: Extremo derecho del menú de navegación.
- Accesibilidad: Alto contraste, foco keyboard visible.

## 5. Acciones Inmediatas (Para Code Mode)
1. Crear carpetas `es` y `en`.
2. Mover y limpiar `index.html` y `index.en.html`.
3. Crear el nuevo `index.html` raíz.
4. Modificar `css/styles.css` o el HTML para añadir el styleswitcher.
5. Crear `js/i18n.js`.
