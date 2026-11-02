# eBook interactivo Código Ético del Psicólogo — EDUPSIC

Paquete listo para alojar en GitHub Pages con subdominio personalizado:

https://codigoetico.edupsic.com/

## Archivos

- `index.html`: eBook completo en una sola página HTML (texto original escaneado e imágenes integradas, lector y resaltador).
- `CNAME`: nombre exacto del subdominio para GitHub Pages.
- `.nojekyll`: indica a GitHub Pages que publique los archivos estáticos directamente.
- `favicon.svg`: icono del navegador.

## Publicación en GitHub

1. En GitHub, bajo la cuenta `eriobeth-art`, crea un repositorio denominado `ebook-codigo-etico` (o usa un repositorio exclusivo nuevo para este eBook).
2. Sube **todos los archivos de esta carpeta** a la raíz (no subas la carpeta contenedora). Confirma los cambios.
3. En el repositorio, abre **Settings > Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**, rama **main** y carpeta **/(root)**. Guarda.
5. En **Custom domain**, establece `codigoetico.edupsic.com` y guarda. Si GitHub crea o modifica el archivo `CNAME`, comprueba que contenga exclusivamente `codigoetico.edupsic.com`.
6. **Antes de apuntar DNS al sitio**, confirma que el dominio personalizado se haya guardado en GitHub Pages. Es recomendable verificar la propiedad del dominio en GitHub (configuración de cuenta > Pages).

## DNS en Squarespace Domains

1. Entra en Squarespace Domains > `edupsic.com` > DNS > DNS Settings > Custom Records > Add record.
2. Añade el registro:
   - Tipo: **CNAME**
   - Nombre / Host: **codigoetico**
   - Data / Destino: **eriobeth-art.github.io**
   - TTL: automático o 1 hora (según opciones disponibles)
3. Guarda. **No uses** `https://`, `http://`, ni `/ebook-codigo-etico` en Data.
4. No cambies los registros `@`, `www` ni otros subdominios de EDUPSIC.
5. Regresa a **Settings > Pages**: cuando DNS y certificado estén listos, activa **Enforce HTTPS**.

Dirección pública prevista: https://codigoetico.edupsic.com/
URL temporal del repositorio, antes de asignar el dominio: https://eriobeth-art.github.io/ebook-codigo-etico/

La propagación DNS puede demorar hasta 24 horas y el certificado HTTPS puede tardar más. No se ha configurado el dominio ni se ha publicado el sitio desde este paquete.

## Uso

- En computador, usa el gesto de arrastre desde una esquina inferior del libro para pasar hoja.
- Zoom: abre la página mediante «Ampliar» y usa sus controles.
- El resaltador guarda trazos en el almacenamiento local del navegador de cada dispositivo; no sincroniza entre alumnos ni equipos.
- Las fotografías externas pueden necesitar conexión a Internet.

## Advertencia editorial

El contenido incluye una reproducción del Código Ético del Psicólogo, Sociedad Mexicana de Psicología / Editorial Trillas (2010). Antes de subirlo a un repositorio público o compartir el enlace, comprueba que cuentes con autorización para reproducir y distribuir el material. El paquete no acredita ni sustituye ese permiso.

## Verificaciones

- El `CNAME` en el repositorio y el dominio configurado en Pages deben coincidir.
- El DNS CNAME debe apuntar a `eriobeth-art.github.io`, **no** al dominio raíz `edupsic.com` ni a una ruta de GitHub.
- Si Google Chrome bloquea acceso al archivo local, prueba el sitio a través de GitHub Pages.

Guías oficiales:
- GitHub Pages: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
- Squarespace: https://support.squarespace.com/hc/en-us/articles/31119879125645-DNS-records-for-web-hosting
