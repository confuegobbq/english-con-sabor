# English con Sabor

Sitio web de English con Sabor: clases de inglés online para familias latinas en Estados Unidos.

Es un sitio estático (HTML + CSS, sin frameworks ni build), pensado para publicarse en Cloudflare Pages.

## Estructura

Todo lo que se publica está en `public/`:

- `index.html`: la landing.
- `styles.css`: estilos con los colores y tipografías del manual de marca.
- `img/`: logo (rodaja) y, cuando estén, las fotos.
- `robots.txt`, `sitemap.xml`: para Google.
- `_headers`: cabeceras de seguridad y caché para Cloudflare.
- `404.html`: página de error.

## Publicar en Cloudflare Pages

1. En Cloudflare: Workers & Pages → Create → Import a repository.
2. Elegir este repositorio.
3. Build command: vacío. Deploy command: `npx wrangler deploy` (lee `wrangler.jsonc`).
4. Deploy. Cada push a `main` se publica solo.



## Pendientes antes de publicar (buscar `TODO` en el código)

- Fotos de Astrid: `img/astrid-hero.jpg` (4:5) e `img/astrid.jpg` (cuadrada), en JPG o WebP de menos de 250 KB.
- Imagen para compartir: `img/og-image.jpg` (1200×630).
- Testimonios reales, con permiso de cada familia.
- Precios, cantidad y duración de clases, descuento del Plan Familia.
- Número de WhatsApp, email, plataforma de videollamada, medios de pago, años de experiencia.
- Dominio definitivo: reemplazar `englishconsabor.com` en `index.html`, `robots.txt` y `sitemap.xml`.
