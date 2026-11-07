# Sitio web GUZFESA Servicios S.R.L.

Sitio estático de una sola página. Incluye una portada con paneles animados, una franja de pilares en movimiento y un carrusel de servicios. También tiene alquiler, galería con visor de fotos y formulario de contacto.

No necesita instalación ni servidor. Solo usa HTML, CSS y JavaScript.

## Contenido

```
index.html      → la página completa (estilos y scripts incluidos)
images/         → fotos y logos
README.md       → este archivo
```

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `guzfesa-web`). Puede ser público.
2. Sube **el contenido de esta carpeta**: `index.html`, la carpeta `images` y este `README.md`.
   - Desde la web: **Add file › Upload files**, arrastra todo y luego haz clic en **Commit changes**.
3. Ve a **Settings › Pages**.
4. En **Build and deployment › Source** elige **Deploy from a branch**.
5. En **Branch** elige `main` y la carpeta `/ (root)`, y haz clic en **Save**.
6. Espera uno o dos minutos. El sitio quedará en:
   `https://TU-USUARIO.github.io/guzfesa-web/`

Para usar un dominio propio (por ejemplo `www.guzfesa.com`), configúralo en **Settings › Pages › Custom domain** y apunta el DNS del dominio a GitHub Pages.

## Formulario de contacto

GitHub Pages no procesa formularios. Por eso, al enviar, el formulario abre la aplicación de correo del visitante con un mensaje ya armado para **guzfesaserviciossrl@hotmail.com**.

Si prefieres recibir los mensajes sin que el visitante use su correo, puedes conectar un servicio como Formspree:

1. Crea un formulario en el servicio y copia su URL.
2. En `index.html`, busca `<form id="contactForm"` y agrega `action="URL-DEL-SERVICIO" method="POST"`.
3. En el script al final del archivo, borra el bloque que empieza con `form.addEventListener('submit'`.

## Editar textos o fotos

- Los textos están en `index.html` y se pueden editar con cualquier editor de texto.
- Para cambiar una foto, reemplaza el archivo en `images/` y mantén el mismo nombre.
