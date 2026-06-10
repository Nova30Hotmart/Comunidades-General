# Comunidades Hotmart — Landing de revelación

Sitio estático. Sin build. Solo archivos.

## Estructura
- index.html
- favicon.svg
- og.png  (1200x630, para compartir)
- assets/fonts, assets/logos, assets/orbs

## Publicar en Vercel (recomendado: GitHub + Vercel)
1. Crea un repo nuevo (o una carpeta nueva en tu repo de hotmartcomunidades) y sube estos archivos respetando la estructura.
2. En Vercel: New Project -> importa el repo. Framework Preset: "Other" (estático). Root: la carpeta de este proyecto. Deploy.
3. Domains -> agrega el subdominio: info.hotmartcomunidades.com
4. En tu DNS crea un CNAME:  info  ->  cname.vercel-dns.com
5. Espera la verificación (suele ser minutos) y listo.

## Importante
- Si el subdominio NO es info.hotmartcomunidades.com, edita en index.html las 3 etiquetas que tienen la URL (og:url, og:image, twitter:image).
- El og.png debe quedar accesible en  https://info.hotmartcomunidades.com/og.png

## Alternativa rápida (sin git)
- Instala Vercel CLI:  npm i -g vercel
- Dentro de esta carpeta:  vercel  (sigue el wizard) y luego  vercel --prod
