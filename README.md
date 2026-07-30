# Aeral — Sitio web

Landing page de Aeral: limpieza profesional de fachadas mediante drones.
Sitio estático (HTML + CSS + JS en un solo archivo). No necesita build ni servidor.

## Estructura

```
aeral-web/
├── index.html          ← la página completa
├── assets/             ← logos, fotos y video
│   ├── logo_dark.png
│   ├── logo_white.png
│   ├── dron.jpg
│   ├── dron2.jpg
│   ├── dron3.jpg
│   ├── demo.mp4
│   └── demo_poster.jpg
└── README.md
```

## Publicar en GitHub y Vercel

### 1) Subir a GitHub (opción sencilla, desde el navegador)

1. Entra a https://github.com/new y crea un repositorio nuevo (por ejemplo `aeral-web`). Déjalo **Public** o **Private**, da igual.
2. En la página del repo vacío, haz clic en **uploading an existing file**.
3. Arrastra **todo el contenido de esta carpeta** (el archivo `index.html`, la carpeta `assets/` y este `README.md`). Importante: sube el contenido, no la carpeta `aeral-web` metida dentro de otra.
4. Abajo, haz clic en **Commit changes**.

### 2) Conectar con Vercel

1. Entra a https://vercel.com y regístrate con tu cuenta de GitHub.
2. Haz clic en **Add New → Project**.
3. Elige el repositorio `aeral-web` y haz clic en **Import**.
4. No cambies nada (Vercel detecta que es un sitio estático). Haz clic en **Deploy**.
5. En un minuto tendrás una URL tipo `aeral-web.vercel.app`. Cada vez que subas cambios a GitHub, Vercel actualiza el sitio solo.

### 3) (Después) Conectar tu dominio

Cuando tengas el dominio (p. ej. `aeral.mx`): en Vercel, entra al proyecto → **Settings → Domains** → agrega el dominio y sigue las instrucciones de DNS.
Al hacerlo, actualiza también estas líneas dentro de `index.html` (están al inicio, en el `<head>`) para que apunten a tu dominio real:

- `<link rel="canonical" href="https://aeral.mx/">`
- `<meta property="og:url" content="https://aeral.mx/">`

## Cambiar contenido más adelante

- **Fotos / video:** reemplaza los archivos dentro de `assets/` conservando el mismo nombre, o cambia la ruta en `index.html`.
- **Textos, teléfonos, correo:** todo está en `index.html`. El correo (`aeralmx@gmail.com`) y los WhatsApp `(55) 4922 6577` y `(55) 6707 5883` aparecen en la sección de contacto y en el pie de página.
- **Formulario:** al enviarlo, arma el mensaje y lo abre en WhatsApp del `(55) 4922 6577`. No requiere servidor.
