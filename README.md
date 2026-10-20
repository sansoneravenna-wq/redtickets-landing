# RedTickets — Landing Web

## Cómo cargar
1. Subí TODO el contenido de esta carpeta (manteniendo la estructura) a la raíz del dominio (o subcarpeta).
2. El archivo principal es `redtickets-landing.html`. Renombralo a `index.html` si va a la raíz.
3. Todos los paths son relativos — funciona en cualquier hosting estático (Vercel, Netlify, S3, Cloudflare Pages, hosting tradicional, etc.).

## Estructura
- `redtickets-landing.html` — archivo principal (260 KB, 7150 líneas)
- `redtickets-logo-{black,orange,white}.png` — logos de RedTickets
- `team/` — 27 fotos del equipo (avatares circulares centrados)
- `drone/` — 4 videos aéreos + posters JPG
- `empresariales/` — recursos de la sección Eventos Empresariales
  - `v1.mp4 ... v4.mp4` — videos de los pasos
  - `2-invitaciones.jpg ... 8-personal.jpg` — imágenes paso a paso (algunas son placeholders)
  - `gallery/g01-g32 (.mp4 + .jpg)` — galería de Reels y Highlights (31 videos, sin click, autoplay loop)
- `media/sobre-nosotros-closer.{mp4,jpg}` — video closer de Sobre Nosotros (104 segundos, autoplay muted loop)
- `gallery/` — imágenes del marquee del home
- `events/` — banner de eventos (ver nota abajo)
- `logos/` — 47 logos de clientes/productores (PNG transparente blanco)

## Notas para el programador
- Todos los videos usan `autoplay muted loop playsinline preload="metadata"` — funcionan en todos los browsers modernos.
- Sin backend ni framework: solo HTML/CSS/JS plano.
- El sitio tiene 5 "páginas" via hash routing: `#home`, `#sobre-nosotros`, `#marketing`, `#empresariales` (página separada existe), `#ayuda`. El menú activo es: RedTickets · Sobre Nosotros · Marketing · Ayuda.
- Página Ayuda tiene tabs: `#ayuda/clientes` y `#ayuda/productores`.

## Assets que pueden necesitar mejora
- `empresariales/{2-invitaciones,3-formulario,4-reportes,6-etiquetas}.jpg` son placeholders usando frames de la galería. Idealmente reemplazar con fotos reales del equipo en acción para cada paso.
- `events/all-banners.jpg` es una página entera del PDF EcosistemaRT con los banners. Idealmente extraer cada banner por separado (15 banners). El HTML referencia: `events/cosquin-rock.jpg`, `events/no-te-va-gustar.jpg`, `events/lali.jpg`, `events/la-vela-puerca.jpg`, `events/la-renga.jpg`, `events/gran-premio-ramirez.jpg`, `events/maria-becerra.jpg`, `events/placido-domingo.jpg`, `events/venta-entradas-uy-arg.jpg`, `events/fundamentalistas.jpg`, `events/fiesta-chacra.jpg`, `events/cerveza-paysandu.jpg`, `events/criolla.jpg`, `events/festival-independencia-florida.jpg`, `events/artigas-carnaval.jpg`.

## Contacto
Para cualquier consulta sobre los assets originales, contactar al equipo de Marketing de RedTickets.
