# Marali Gráficas

Landing page estática para Marali Gráficas, imprenta y emprendimiento familiar de Villa Alemana.

## Vista pública

GitHub Pages publica automáticamente la rama `main`:

<https://sebmunz.github.io/marali_graficas/>

## Ejecutar localmente

No requiere instalación ni proceso de compilación. Desde la raíz del repositorio:

```powershell
python -m http.server 8765 --bind 127.0.0.1
```

Luego abre <http://127.0.0.1:8765/>.

## Estructura

- `index.html`: contenido y estructura semántica.
- `css/styles.css`: sistema visual y responsive.
- `js/scripts.js`: menú móvil, header y animaciones progresivas.
- `assets/img`: logotipo, imágenes y recursos gráficos.
- `assets/img/portfolio/real-work`: destino para fotografías definitivas del portafolio.

## Contenido pendiente de confirmar

Antes de considerar la landing definitiva, validar con Marali:

- catálogo exacto de servicios y materiales;
- historia del emprendimiento familiar;
- imágenes de trabajos reales;
- enlaces oficiales de redes sociales;
- disponibilidad, cobertura, plazos y condiciones de entrega.

Las imágenes actuales del portafolio están identificadas visualmente como referenciales.

## Publicación

GitHub Pages está configurado para publicar la raíz de `main`. Cada push a esa rama genera una nueva versión del sitio.
