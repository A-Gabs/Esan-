# Panel de Simuladores · Sistemas Operativos

Un único archivo (`index.html`) que reúne los 4 simuladores de Sistemas
Operativos. No hay carpetas ni archivos sueltos: todo el código de cada
simulador está embebido dentro de este HTML, así que puedes subirlo tal
cual a GitHub sin preocuparte por rutas rotas.

**Gestión de memoria**
- FIFO — Reemplazo de páginas
- LFU — Reemplazo de páginas

**Planificación de CPU**
- Prioridad no expropiativo
- Round Robin

Cada simulador corre aislado dentro de un `iframe` (vía `srcdoc`), así que
ninguno interfiere con los otros aunque compartan nombres de funciones o
variables internamente.

## Cómo subirlo a GitHub (por la web, sin terminal)

1. Entra a tu repositorio en GitHub.
2. Si tienes algo subido de antes (el .zip, carpetas viejas), bórralo para
   que no quede basura.
3. Click en **"Add file" → "Upload files"**.
4. Arrastra únicamente el archivo `index.html`.
5. Commit directo a `main`.

## Publicarlo con GitHub Pages

1. **Settings → Pages**.
2. En "Source", elige la rama `main` y la carpeta `/ (root)`.
3. Guarda y espera 1-2 minutos.
4. Tu panel queda en: `https://TU_USUARIO.github.io/TU_REPO/`

## Notas

- Como todo vive en un solo archivo, no hay riesgo de rutas rotas
  (`algoritmos/fifo.html`, etc.) ni de subir el zip por error.
- Enlaces directos: `index.html#fifo`, `#lfu`, `#prioridad`, `#roundrobin`
  abren cada simulador directamente.
- Si necesitas editar un simulador puntual, es más práctico trabajar sobre
  los archivos sueltos originales y luego volver a generar el `index.html`
  unificado, en vez de editar el HTML embebido en base64 a mano.
