# Aeral — Sitio web

Landing page de Aeral: limpieza profesional de fachadas mediante drones.
Es **un solo archivo** (`index.html`) con todo incluido: textos, estilos, fotos, video y logos.
No necesita build, ni servidor, ni carpeta de imágenes. Se abre y funciona en cualquier lado.

## Publicar en GitHub y Vercel

### 1) Subir a GitHub (desde el navegador)
1. Entra a https://github.com/new y crea un repositorio nuevo (p. ej. `aeral-web`).
2. En el repo vacío, haz clic en **uploading an existing file**.
3. Arrastra el archivo **`index.html`** (y si quieres, este `README.md`). Nada más: no hay carpetas que subir.
4. Haz clic en **Commit changes**.

### 2) Conectar con Vercel
1. Entra a https://vercel.com y regístrate con tu cuenta de GitHub.
2. **Add New → Project** → elige el repo `aeral-web` → **Import**.
3. No cambies nada (Vercel detecta que es un sitio estático). Haz clic en **Deploy**.
4. En un minuto tendrás una URL tipo `aeral-web.vercel.app`. Cada cambio que subas a GitHub se actualiza solo.

### 3) (Después) Conectar tu dominio
Cuando tengas el dominio (p. ej. `aeral.mx`): Vercel → proyecto → **Settings → Domains** → agrégalo y sigue las instrucciones de DNS.
Luego actualiza estas dos líneas dentro de `index.html` (al inicio, en el `<head>`) para que apunten a tu dominio:
- `<link rel="canonical" href="https://aeral.mx/">`
- `<meta property="og:url" content="https://aeral.mx/">`

## Datos de contacto en la página
- Correo: `aeralmx@gmail.com`
- WhatsApp: `(55) 4922 6577`
El botón **Solicitar cotización** abre el formulario de Google (https://forms.gle/zSQ5pXqJb6WkbWW29) en una pestaña nueva.

## Cambiar textos o el correo/teléfono
Todo está en `index.html`. Ábrelo con cualquier editor de texto, busca lo que quieras cambiar y guárdalo.

> Nota: como las fotos y el video van incrustados en el archivo, para reemplazarlos por material propio más adelante es más práctico que me pases las nuevas imágenes y te regenero el `index.html`. Toma un momento.
