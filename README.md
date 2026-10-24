# Córdoba 360 · Primera entrega

Plataforma web turística del departamento de Córdoba, Colombia. Curso Desarrollo Web I, Universidad de Córdoba (2026-II). Autor: Alex Arrieta.

Esta primera entrega cubre la **semántica estructural, la maquetación responsive y el versionamiento**: HTML5 y CSS3, sin interactividad compleja.

## Páginas

| Archivo | Contenido (según los mockups) |
| --- | --- |
| `index.html` | Inicio: hero, destinos populares y experiencias |
| `destinos.html` | Listado de destinos por categoría (playas, pueblos, naturaleza) |
| `experiencias.html` | "Vive experiencias inolvidables": 6 categorías |
| `informacion.html` | Conoce Córdoba: historia, cifras, consejos de viaje |
| `san-antero.html` | Ficha de destino: ubicación, clima, galería y mapa |
| `contacto.html` | Formulario de contacto y canales de atención |
| `registro.html` | Registro e inicio de sesión |

## Estructura de carpetas

```
cordoba360/
├── index.html, destinos.html, experiencias.html, informacion.html,
│   san-antero.html, contacto.html, registro.html
├── css/
│   └── styles.css      ← hoja de estilos externa única
└── img/                ← imágenes optimizadas en .webp y .jpg
```

## Cumplimiento de requisitos

**1. Estructura semántica (HTML5)**
- `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>` y `<footer>` en todas las páginas, con muy pocos `div` (solo como envoltorios de diseño).
- Formularios con validación nativa: `required`, `pattern`, `minlength`/`maxlength`, `min`, `max`, `type="email"`, `type="date"`, `type="tel"`, `type="number"`.
- Metadatos en `<head>`: `charset`, `viewport`, `title`, `description`, `theme-color` y Open Graph.
- Multimedia: `<picture>` con WebP y respaldo JPG, `loading="lazy"`, logo en `<svg>` en línea y favicon SVG.

**2. Maquetación y diseño adaptativo (CSS3)**
- Estilos externos en `css/styles.css`, organizados por módulos.
- **CSS Grid** para la macro-estructura (`.pagina`: header / main / footer), el pie de página y las rejillas de tarjetas.
- **Flexbox** para la barra de navegación, las tarjetas, los botones y la barra de herramientas.
- Mobile First con **tres breakpoints**: tablet (`min-width: 600px`), escritorio (`min-width: 1024px`) y escritorio amplio (`min-width: 1280px`).
- Menú móvil y mega menú de Destinos hechos solo con CSS (checkbox, `:hover` y `:focus-within`).
- Recursos externos vía CDN: tipografía **Inter** (Google Fonts) e iconos **Font Awesome 6.5.1** (cdnjs).

## Cómo verlo

Abre `index.html` en el navegador. También puedes usar la extensión *Live Server* de VS Code.

## Subirlo a GitHub (entrega)

```bash
git init
git add .
git commit -m "Estructura semántica HTML5 de las páginas de Córdoba 360"
git branch -M main
git remote add origin https://github.com/<tu-usuario>/cordoba360.git
git push -u origin main
```

Se recomienda hacer commits descriptivos por avance, por ejemplo: "Maquetación del inicio con Grid y Flexbox", "Breakpoints para tablet y móvil", "Formularios con validación nativa".

Para publicarlo con GitHub Pages: *Settings → Pages → Branch: main / root*.

## Referencias

Colombia Travel. (s. f.). *Descubre Colombia a través de sus regiones*. Recuperado el 25 de agosto de 2026, de https://colombia.travel/es/donde-ir

Escuela de Programación. (s. f.). *Diferencia entre HTML, CSS y JavaScript: guía visual para novatos*. Recuperado el 25 de agosto de 2026, de https://escueladeprogramacion.net/blog/diferencia-entre-html-css-y-javascript-guia-visual-para-novatos

GitHub. (s. f.). *GitHub Education*. Recuperado el 25 de agosto de 2026, de https://github.com/education?locale=es-419

Gobernación de Córdoba. (2021). *Turismo*. Recuperado el 25 de agosto de 2026, de https://www.cordoba.gov.co/publicaciones/18/turismo/

Ministerio de Comercio, Industria y Turismo. (s. f.). *Portal de Información Turística de Colombia*. Recuperado el 25 de agosto de 2026, de https://portucolombia.mincit.gov.co/

Miro. (2023, 20 de marzo). *Wireframe: Qué es, cómo hacerlo y ejemplos*. Recuperado el 25 de agosto de 2026, de https://miro.com/es/wireframe/que-es-wireframe/

## Créditos de imágenes

Fotografías tomadas del material visual del proyecto (mockups del documento Córdoba 360) y de la carpeta de imágenes de referencia del autor. Uso académico.
