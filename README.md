# Padel Galaxy (proyecto_final_Bootstrap)

Proyecto web estático (HTML + Bootstrap) que maqueta la web de **Padel Galaxy**: una landing y una página de catálogo de palas.

## Vista general

- **Tipo**: sitio web estático (sin backend)
- **Tecnologías**:
  - HTML5
  - Bootstrap (CSS/JS en `dist/`)
  - Bootstrap Icons (CDN)
  - Assets locales (imágenes en `img/`)

## Páginas

- `index.html`
  - Landing (hero) + secciones de “Pistas destacadas” y “Últimas novedades”.
- `tienda.html`
  - Catálogo de palas con sidebar de filtros (UI) y grid de productos.

## Estructura del proyecto

- `index.html`
- `tienda.html`
- `dist/`
  - `css/`: build de Bootstrap (`bootstrap.css`, `bootstrap.min.css`, etc.)
  - `js/`: build de Bootstrap (`bootstrap.bundle.min.js`, etc.)
- `scss/`
  - Fuentes SCSS de Bootstrap (para personalización/compilación si se desea)
- `img/`
  - Imágenes usadas por las páginas
- `Capturas Adobe/`
  - Capturas/exportaciones del diseño (referencia)

## Cómo ejecutarlo

Al ser un proyecto estático, puedes abrirlo directamente o servirlo con un servidor local.

### Opción A: abrir en el navegador

1. Abre `index.html` en tu navegador.

### Opción B: servidor local (recomendado)

- Con VS Code: extensión **Live Server** y abrir `index.html`.
- Con cualquier servidor estático:
  - Sirve la carpeta del proyecto y entra a `/index.html`.

## Notas técnicas

- El proyecto carga Bootstrap desde `dist/css/bootstrap.css` y `dist/js/bootstrap.bundle.min.js`.
- Los iconos se cargan desde CDN:
  - `https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css`
- No hay `package.json` ni pipeline de build configurado en el repo; `scss/` está incluido para referencia/personalización, pero **no se compila automáticamente**.

## Ideas de mejora (opcional)

- Añadir más páginas reales a los enlaces del navbar (contacto, reservas, login, carrito).
- Implementar filtros y carrito con JavaScript.
- Añadir un pipeline de compilación SCSS (npm + sass) para personalizar Bootstrap de forma reproducible.

## Licencia

No se especifica licencia en el repositorio. Si quieres que sea reutilizable, añade un archivo `LICENSE` (por ejemplo MIT) e indica la autoría.
