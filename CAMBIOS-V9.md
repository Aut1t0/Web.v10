# Cambios v9 — Olivícola Luján

- Eliminado el video del hero para evitar la primera reproducción automática.
- El video de la sección **Origen / Maipú, Mendoza** queda en `autoplay`, `muted`, `loop` y `playsinline`, y el JavaScript intenta reproducirlo al cargar.
- Eliminados del HTML los overlays SVG y tooltips de los mapas de Argentina y mercados internacionales; quedan únicamente los mapas base y sus listas laterales.
- Eliminado el mapa mundial de puntos usado para elegir idioma.
- Reemplazada la ventana modal de idioma por una sección visible **00 / IDIOMA** con tres opciones directas: Español, English y Português.
- El botón de idioma del encabezado ahora lleva a la sección de idioma.
- La selección de idioma cambia el idioma global del sitio y marca visualmente la opción activa.
- El ZIP final se genera con `index.html` directamente en la raíz para facilitar la apertura o publicación en GitHub Pages/hosting estático.
