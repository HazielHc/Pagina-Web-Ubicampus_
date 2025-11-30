# Documentación: `Inicio.html`

## Resumen

Página de inicio de la plataforma "Ubicampus". Presenta la cabecera con logo y enlaces externos, una sección hero con imagen de fondo y títulos principales, un bloque informativo "Sobre Ubicampus" y un pie de página simple.

## Recursos incluidos

- TailwindCSS (CDN): para utilidades de estilo y diseño responsivo.
- Google Fonts: familias `Inter` y `Merriweather`.
- Phosphor Icons: iconos usados en la cabecera y footer.

## Estructura del archivo

- `HEAD`: configuración de meta, carga de Tailwind, fuentes e iconos, y configuración de colores/font en `tailwind.config`.
- `HEADER` (cabecera): barra superior fija que contiene:
  - Bloque del logo (enlace a `Inicio.html`).
  - Enlaces externos: Página oficial de la universidad y Moodle.
  - Grupo derecho: botón de acceso/menú con estilo azul.
- `MAIN` (hero): imagen de fondo con gradiente y contenido principal centrado (títulos y lema). Incluye un elemento `#searchFeedback` para mostrar mensajes de error/estado.
- Sección `Sobre Ubicampus`: bloque informativo con descripción de la plataforma.
- `FOOTER`: pie de página con el nombre/marca.

## Comentarios sobre edición

- Para cambiar los colores principales, editar los valores en la sección `tailwind.config` dentro del `head` (claves `ub-blue` y `ub-dark`).
- La imagen de fondo usa `onerror` para cargar una imagen alternativa si falla la ruta local. Reemplazar `src` con la ruta correcta si es necesario.
- Clases utilitarias de Tailwind controlan la responsividad (`md:`) y las animaciones (por ejemplo `animate-bounce`, `fade-in-up`).

## Accesibilidad y buenas prácticas

- Añadir `alt` descriptivos y adecuados a las imágenes; actualmente la imagen principal tiene `alt="University Campus"`.
- Si se añade contenido interactivo (formularios, menús desplegables), asegurar `aria-*` y manejo de foco para navegación por teclado.

## Cómo personalizar rápidamente

1. Cambiar título visible en `<title>` y en el `h1` para adaptar al nombre de su proyecto.
2. Actualizar los enlaces externos (`https://upnay.edu.mx/` y `.../mupen/login/index.php`) a sus destinos reales.
3. Para cambiar tipografía, modificar la carga en Google Fonts y actualizar `fontFamily` en `tailwind.config`.

## Notas finales

El archivo contiene comentarios añadidos en español dentro del HTML para explicar cada bloque. Esta documentación separada proporciona una visión general y pasos rápidos para editar y mantener la página.

Si quieres, puedo:

- Actualizar más páginas del proyecto con comentarios en español.
- Extraer estilos comunes a un archivo CSS separado.
- Preparar una versión imprimible de esta documentación.

---
Archivo generado automáticamente: `Bienvenida/Inicio_documentacion.md`.
