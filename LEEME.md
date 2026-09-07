# Army Forge — publicarlo desde el móvil (sin StackBlitz, sin instalar nada)

Esta carpeta tiene 4 archivos: `index.html` (tu app entera, sin necesidad de
compilar nada — usa React directamente desde internet), `manifest.json` y
dos iconos. Solo tienes que subirlos a GitHub.

## Paso 1 — Crear el repositorio

1. Ve a **https://github.com** en el navegador de tu móvil (o abre la app
   de GitHub) e inicia sesión / crea una cuenta gratis
2. Pulsa el **"+"** de arriba → **"New repository"**
3. Ponle un nombre (por ejemplo `army-forge`), márcalo como **Public**,
   y pulsa **"Create repository"**

## Paso 2 — Subir los 4 archivos

1. Dentro del repositorio recién creado, busca el enlace
   **"uploading an existing file"** (aparece en la pantalla inicial del repo vacío)
2. Pulsa ahí, y selecciona los 4 archivos de esta carpeta
   (`index.html`, `manifest.json`, `icon-192.png`, `icon-512.png`) —
   tu navegador te dejará elegirlos desde donde hayas guardado el zip
3. Baja del todo y pulsa **"Commit changes"**

## Paso 3 — Activar GitHub Pages

1. Ve a la pestaña **"Settings"** del repositorio
2. En el menú lateral, busca **"Pages"**
3. En "Branch", elige **"main"** y la carpeta **"/ (root)"** → **"Save"**
4. Espera 1-2 minutos. Te aparecerá una URL tipo:
   `https://tu-usuario.github.io/army-forge/`

## Paso 4 — Generar el APK

1. Ve a **https://www.pwabuilder.com**
2. Pega la URL del paso anterior
3. Pestaña **Android** → **"Generate Package"**
4. Descarga el `.apk`

## Nota importante

Este `index.html` funciona de una forma distinta a la mayoría de webs:
en vez de venir "precompilado", carga React directamente desde internet
la primera vez que se abre y traduce el código al vuelo en el propio
navegador. Esto significa que **necesita conexión a internet la primera
vez** que se abre en cada dispositivo para descargar React (unos 150 KB),
aunque el resto de la app (los datos de las facciones) ya va incluido
en el propio archivo. Para uso normal esto no se nota en nada.
