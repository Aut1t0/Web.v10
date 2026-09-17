# Olivícola Luján — sitio estático

Sitio web estático de Olivícola Luján, preparado para publicarse en **GitHub Pages**.

## Estructura

`index.html` está en la raíz del repositorio y todos los recursos locales se encuentran dentro de `assets/`.

```text
/
├── index.html
├── style.css
├── script.js
├── README.md
├── REFACTOR-REPORT.md
├── .gitignore
└── assets/
    └── imágenes del sitio
```

## Publicar en GitHub Pages

1. Descomprime este ZIP.
2. Crea un repositorio nuevo en GitHub.
3. Sube **el contenido de esta carpeta**, no el ZIP como archivo.
4. Comprueba que `index.html` quede directamente en la raíz del repositorio.
5. En GitHub entra en **Settings → Pages**.
6. En **Build and deployment**, selecciona **Deploy from a branch**.
7. Selecciona la rama `main` y la carpeta `/ (root)`.
8. Guarda la configuración.

GitHub Pages debería publicar el sitio con una URL similar a:

```text
https://TU-USUARIO.github.io/TU-REPOSITORIO/
```

## Ejecutar localmente

Puedes abrir `index.html` directamente para una comprobación rápida. Para una prueba más cercana al entorno de GitHub Pages, usa un servidor local:

```bash
python -m http.server 5500
```

Luego visita `http://127.0.0.1:5500/`.

## Datos locales

La cuenta, el contador de visitas y las valoraciones utilizan `localStorage` del navegador. GitHub Pages puede ejecutar estas funciones, pero los datos no se comparten entre visitantes ni entre dispositivos.

Para cuentas reales, visitas globales y valoraciones compartidas se necesitaría un backend, una base de datos o un servicio externo.


## Versión v8 - mejoras aplicadas

- Numeración consolidada en 01–07 y sección 05 fusionada como “Presencia en el Mercado”, manteniendo `#export` como ancla interna.
- Selector de idioma con mapa mundial interactivo por grupos ES/PT/EN, tooltips y selección accesible por teclado.
- Recalibración de los puntos problemáticos del mapa argentino (`CABA` y `Chubut`) y ajuste fino de Argentina/Chile en el mapa mundial.
- Catálogo validado contra las 8 tarjetas reales generadas por JavaScript.
- CSS saneado para usar una sola definición por componente/breakpoint y mejorar el comportamiento en 360/390/768/1024/1280/1440 px.
- Video en el hero reutilizando el loop `olive-motion.mp4`, con autoplay/muted/loop/playsinline y poster, manteniendo el video de origen existente.
- Imágenes principales convertidas a WebP de alta calidad y nombres de archivos normalizados para evitar espacios y paréntesis.
- Mejoras de foco, estados activos/neutros y formas de puntos para que la lectura de mapas no dependa solo del color.
