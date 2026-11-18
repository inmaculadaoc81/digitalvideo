

BLOG (/blog):
- Los artículos NO viven en este repositorio: los genera y aprueba el agente
  SEO de Kelatos (Agentes V2 → organización «DigitalVideo», clave digitalvideo)
  y se leen en vivo de la API pública de Kelatos, sin token:
  https://db.affirmatechnology.com/kelatos-api/publico/blog?org=digitalvideo
- api/blog.js + lib/blog.js generan /blog y /blog/<slug> en el servidor.
- api/sitemap.js genera /sitemap.xml (se eliminó el sitemap.xml estático).
- Estilos en assets/blog.css. Enlace «Blog» en el menú (escritorio y móvil) y en el pie.
- vercel.json redirige a la home las URLs antiguas; el blog queda fuera.
- La web principal es www.digitalizarcintas.es (el dominio sin www redirige): canonical, og:url, datos estructurados y robots.txt apuntan a www.
- middleware.mjs excluye /blog (en la práctica Vercel no lo ejecuta en este proyecto estático).
