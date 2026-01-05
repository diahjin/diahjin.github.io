# Cine de fernolv

Pequeña web estática hospedada en **GitHub Pages** que muestra un reproductor de vídeo con varias películas alojadas en Google Drive. [web:157][web:180]

## Cómo funciona

- El sitio se sirve desde el repositorio `fernolv.github.io` usando GitHub Pages.
- El archivo `index.html` usa **Video.js** como reproductor HTML5.
- Las películas están en Google Drive y se cargan mediante enlaces directos del tipo:

`https://drive.google.com/uc?export=download&id=FILE_ID` [web:91][web:213]

## Playlist de películas

En `index.html` hay un array `playlist` en JavaScript con todas las URLs directas de las pelis:

```js
const playlist = [
  "https://drive.google.com/uc?export=download&id=...",
  // más pelis aquí
];
