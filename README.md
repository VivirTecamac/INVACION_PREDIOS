# Predio invadido por lotificadores – Ampliación San Jerónimo

Panel web (compatible con iOS, Android y escritorio) de **Vivir Tecámac S.A. de C.V.**
que muestra el mapa operativo del predio invadido y un botón para iniciar la
navegación GPS en Google Maps (enlace `comgooglemaps://`, para iPhone con la app de Google Maps instalada).

## Estructura

```
.
├── index.html                    # Página principal
├── assets/
│   ├── fondo-panel.jpg           # Fondo del panel lateral
│   └── logo-vivir-tecamac.png    # Logo
├── .nojekyll                     # Evita el procesado de Jekyll en GitHub Pages
├── .gitignore
└── README.md
```

## Ver en local

Abre `index.html` en el navegador (doble clic). No requiere instalación.

## Publicar con GitHub Pages

1. Sube el repositorio a GitHub.
2. En el repositorio: **Settings → Pages**.
3. En *Source* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
4. Espera 1–2 minutos. La URL será:
   `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`

## Actualizar el destino o el mapa

- **Destino GPS:** en `index.html`, cambia las coordenadas del enlace
  `daddr=19.733839,-98.936363`.
- **Mapa:** cambia el valor `mid=` en la URL del `<iframe>` (ID del mapa de Google My Maps).
- **Más destinos:** duplica el bloque `<a class="btn-ruta">…</a>` dentro de `.lista-botones`.

> El mapa de Google My Maps debe estar compartido como **“Cualquier persona con el enlace”**
> para que se vea en la página publicada.
