# Portfolio — Matias Nahuel Sanchez

Portfolio Fullstack Developer + AI Engineer. Sitio estático, sin build.

## Contenido
- `index.html` — el portfolio (autocontenido, funciona offline).
- `CV-Matias-Sanchez.html` — el CV (lo abre el botón "Ver CV online").

## Desplegar en Vercel (vía GitHub)

### 1. Subir a GitHub
1. Creá un repo nuevo en https://github.com/new (ej. `portfolio`), público o privado.
2. Subí estos archivos a la raíz del repo. Dos formas:
   - **Web:** en el repo → "Add file" → "Upload files" → arrastrá `index.html` y `CV-Matias-Sanchez.html` → "Commit changes".
   - **Git (terminal):**
     ```bash
     git init
     git add .
     git commit -m "portfolio"
     git branch -M main
     git remote add origin https://github.com/TU-USUARIO/portfolio.git
     git push -u origin main
     ```

### 2. Desplegar en Vercel
1. Entrá a https://vercel.com y registrate con tu cuenta de GitHub.
2. "Add New..." → "Project" → "Import" el repo `portfolio`.
3. **Framework Preset:** dejá `Other` (es HTML estático, no necesita build).
4. **Build Command:** vacío. **Output Directory:** vacío (raíz).
5. "Deploy". En ~20s tenés tu URL `https://portfolio-xxx.vercel.app`.

Cada push a `main` redepliega solo.

## Notas
- El portfolio es un único HTML; podés subirlo a Netlify o GitHub Pages igual de fácil.
- Para editarlo a futuro conviene volver al archivo fuente `Portfolio Editorial.dc.html` y re-exportar, en vez de tocar `index.html` (está minificado).
