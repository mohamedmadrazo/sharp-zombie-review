# sharp-zombie-review — dashboard de revisión del cliente (SWE / Sharp Zombie)

- `index.html` único; lee `manifest.js` desde GitHub Pages de `swe-sz-media` (o de una rama con `?branch=<rama>` vía jsDelivr).
- Las galerías se rellenan filtrando el manifest por `linea` y `escena`; para una línea nueva añade la sección y el bloque JS siguiendo `#video1` (línea `D_TOKYO_V1`).
- Decisiones: `DEC`, `LBL` y `order` deben ir a la par; los contadores usan `order.length`.
- Verificación: `node -e` para sintaxis del script principal y captura con Playwright (`/opt/node22/lib/node_modules/playwright`, Chromium en `/opt/pw-browsers`) sirviendo el manifest en local.
- Procedimiento de producción de vídeos: skill `comercial-pipeline` y `docs/pipeline_comercial.md` en `swe-sz-media`.
