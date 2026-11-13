# DIW - Diseño de Interfaces Web 🎨

Repositorio de prácticas, actividades y proyectos del módulo **Diseño de Interfaces Web (DIW)**, perteneciente al 2º curso del Ciclo Formativo de Grado Superior en **Desarrollo de Aplicaciones Web (DAW)**.

---

## 📁 Proyectos y Unidades

### 📚 Unidad 4: `trastienda-ud4` — La Trastienda

Prototipo de tienda online de libros especializada en novela negra y *thriller*, diseñado con un enfoque **Mobile-First**, haciendo énfasis en la semántica HTML5, accesibilidad web (A11y) y maquetación moderna con CSS3.

#### 📄 Páginas implementadas

- **`index.html` (Página de Inicio / Catálogo)**:
  - Cabecera con logotipo y botones de acción rápida (búsqueda y menú).
  - Sección de **Novedades** estructurada mediante artículos con portada, título, autor y precio.
  - Sección de **Recomendados** con opción directa de «Añadir a la cesta».
  - Barra de navegación inferior fija para acceso rápido entre secciones de la app.

- **`carrito.html` (Mi Cesta)**:
  - Resumen de artículos seleccionados con detalles (título, autor, formato).
  - Controles de cantidad interactivos (`−` / `+`) y visualización de precios.
  - Desglose de costes (subtotal, gastos de envío y total).
  - Botón de llamada a la acción (CTA) para **Tramitar pedido**.

### 🎴 Proyecto personal: `libreria-manga` — Librería Manga

Maqueta móvil de una librería temática de manga construida solo con HTML5 y CSS nativo (sin preprocesadores, frameworks, Tailwind ni JavaScript), siguiendo la sesión 04 del curso: variables CSS, colores `oklch()` y anidamiento nativo. Viewport objetivo: 393 × 852 px.

#### 📄 Páginas implementadas

- **`index.html` (Home)**:
  - Cabecera con el título de la librería.
  - Cuatro tarjetas `article.card` con título (`h2`), autor, precio y botón de compra.
  - Navegación inferior con tres enlaces (Inicio, Buscar, Favoritos); Inicio lleva `aria-current="page"`.

#### 🎨 Sistema de diseño

- **Tokens en `:root`**: escalas primaria (50–900) y neutra, tokens semánticos (`--bg-page`, `--bg-card`, `--text-main`, `--text-muted`, `--border-subtle`, `--brand`, `--brand-hover`) y el acento `--color-accent`.
- **Colores en oklch**: cada color hex lleva en un comentario su equivalente `oklch(L C H)`, calculado con un script y comprobado.
- **CSS con anidamiento nativo**: máximo tres niveles, sin `!important` ni selectores por `#id`.

---

## 🛠️ Tecnologías y Buenas Prácticas

- **HTML5 Semántico**: Empleo de elementos estructurales nativos (`<header>`, `<main>`, `<section>`, `<article>`, `<nav>`, `<dl>`, `<dt>`, `<dd>`) que garantizan un árbol DOM limpio y comprensible.
- **Accesibilidad (a11y)**:
  - Atributos `aria-label` y `aria-labelledby` para identificar regiones accesibles y controles sin texto visible.
  - Indicador de estado de navegación activa mediante `aria-current="page"`.
  - Descripciones textuales precisas en el atributo `alt` de todas las imágenes.
- **CSS3 Moderno y Mobile-First**:
  - Enfoque adaptable optimizado para dispositivos móviles (`max-width: 480px`).
  - Maquetación flexible con **Flexbox** para la alineación de listas, cabeceras y tarjetas.
  - Uso de selectores modernos como `:has()` para estilos contextuales.
  - Barra de navegación inferior fija (`position: fixed`) con compensación de scroll (`padding-bottom`).
  - Tipografía del sistema (`system-ui`) para máxima velocidad de carga y consistencia en el dispositivo del usuario.
- **Gráficos Vectoriales (SVG)**:
  - Portadas e ilustraciones ligeras y escalables sin pérdida de resolución.

---

## 📂 Estructura de Directorios

```text
DIW/
├── README.md
├── trastienda-ud4/
│   ├── index.html              # Portada y catálogo de la tienda
│   ├── carrito.html            # Vista del carrito de la compra
│   ├── css/
│   │   └── estilos.css         # Hoja de estilos compartida
│   └── img/                    # Portadas de libros en formato SVG
│       ├── el-enigma-de-la-habitacion-622.svg
│       ├── el-mentiroso.svg
│       ├── el-silencio-de-la-ciudad-blanca.svg
│       ├── la-chica-del-tren.svg
│       ├── la-paciente-silenciosa.svg
│       ├── reina-roja.svg
│       └── todo-esto-te-dare.svg
└── libreria-manga/
    ├── index.html              # Pantalla Home (catálogo de manga)
    ├── css/
    │   └── estilos.css         # Tokens en :root y estilos con anidamiento nativo
    └── img/                    # Carpeta preparada (vacía por ahora)
```

---

## 🚀 Cómo visualizar el proyecto

1. **Clonar el repositorio** (o descargar los archivos):
   ```bash
   git clone https://github.com/gregoriolopeez/DIW.git
   ```
2. **Abrir en el navegador**:
   - Navega hasta la carpeta `trastienda-ud4/` y haz doble clic sobre [index.html](file:///c:/Users/grego/Documents/2DAW/DIW/trastienda-ud4/index.html) o [carrito.html](file:///c:/Users/grego/Documents/2DAW/DIW/trastienda-ud4/carrito.html).
   - Proyecto personal: abre [libreria-manga/index.html](libreria-manga/index.html).
   - Alternativamente, puedes usar una extensión como **Live Server** en VS Code para recarga en vivo en un entorno de desarrollo local.

---

## 👤 Autor

- **Gregorio López** — *2º DAW (Diseño de Interfaces Web)*

