# Marali Gráficas

Sitio estático para Marali Gráficas, microempresa familiar de producciones gráficas de Villa Alemana.

## Sitio

- `index.html`: landing comercial y contacto.
- `trabajos.html`: portafolio ampliado.
- `css/styles.css`: identidad visual y diseño responsive.
- `js/scripts.js`: menú móvil y mejoras progresivas.
- `assets/img/trabajos`: fotografías seleccionadas y optimizadas para web.
- `_headers`: cabeceras de seguridad para Cloudflare Pages.
- `404.html`: recuperación de rutas inválidas.

La carpeta local `FOTOS/` contiene material fuente y está excluida de Git. Solo deben publicarse derivados revisados y optimizados.

## Desarrollo local

No requiere instalación ni compilación:

```powershell
python -m http.server 8765 --bind 127.0.0.1
```

Abrir <http://127.0.0.1:8765/>.

## Preview actual

GitHub Pages: <https://sebmunz.github.io/marali_graficas/>

GitHub Pages se utiliza como preview del proyecto. Para publicación comercial se recomienda Cloudflare Pages.

## Publicar en Cloudflare Pages

1. Crear un proyecto en **Workers & Pages → Create → Pages → Import an existing Git repository**.
2. Conectar `SebMunz/marali_graficas`.
3. Usar rama de producción `main`.
4. Framework preset: `None`.
5. Build command: dejar vacío.
6. Build output directory: `/`.
7. Desplegar y comprobar `index.html`, `trabajos.html`, `robots.txt`, `sitemap.xml` y una ruta inexistente.
8. Cuando exista URL definitiva, reemplazar las URLs de GitHub Pages en metadata, `robots.txt` y `sitemap.xml`.

Cloudflare generará previews para ramas y pull requests. Un dominio propio puede agregarse después desde **Custom domains**.

## Revisión antes de publicar

- Confirmar teléfono, correo, redes y autorización de fotografías.
- Revisar desktop, móvil, teclado y menú.
- Ejecutar `node --check js/scripts.js` y `git diff --check`.
- Comprobar que `FOTOS/` sigue ignorada.
- Validar que canonical, Open Graph, sitemap y robots usan el dominio definitivo.
