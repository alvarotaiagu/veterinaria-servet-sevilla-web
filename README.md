# Clínica Veterinaria Servet Sevilla · web

Propuesta de web para la Clínica Veterinaria Servet Sevilla (Av. de Irlanda, 4,
41012 Sevilla). Es una página estática que se genera desde dos archivos de datos.

- **Publicada:** https://alvarotaiagu.github.io/veterinaria-servet-sevilla-web/
  (con `noindex`: no sale en buscadores mientras sea una propuesta).
- **Local:** `node scripts/servir.mjs` → http://127.0.0.1:4191/

## Cambiar algo

1. Datos (horario, teléfonos, servicios, preguntas…): `negocio.json`.
2. Colores, letra y logo: `marca/marca.json` y `marca/*.svg`.
3. Fotos: `media/` con nombre fijo (ver `RESKIN.md` §5).
4. `node scripts/aplicar.mjs` y `node scripts/verificar.mjs --rapido`.

No se edita el HTML a mano: `index.html`, las páginas legales y la 404 se
regeneran desde `fuente/`.

## Datos pendientes

- **NIF** del titular (Servicios Veterinarios Integrales de Sevilla, S. L.): sale
  como `[PENDIENTE]` en el aviso legal y en la política de privacidad.

## Logo

Vectorizado a partir del logo de la cabecera de servetsevilla.es (JPG de
958 × 822 px) con los dos colores exactos de la marca: azul `#027DC4` y rojo
`#D02136`. La cabecera usa la versión horizontal (cruz + SERVET SEVILLA), la
misma composición que el toldo de la fachada. El original y los pasos están en
`_scratch/logo/` (fuera del repo).
