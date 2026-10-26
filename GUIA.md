# Guía de puesta en marcha (una sola vez)

## 1. Subir la web a GitHub
1. Crea una cuenta en github.com si no tienes.
2. Crea un repositorio **público** (por ejemplo `portfolio`).
3. Sube estos archivos y carpetas a la raíz del repositorio: `index.html`, `datos.json` y la carpeta `imagenes/` (con `arte/` y `juegos/`). No hace falta subir `context/` ni esta guía.

## 2. Activar GitHub Pages
1. En el repositorio: **Settings → Pages**.
2. En *Build and deployment*, elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`. Guarda.
3. Al cabo de un minuto, la web estará en `https://TU-USUARIO.github.io/portfolio/`.

## 3. Crear el token de editor
1. GitHub → tu foto → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. *Repository access*: **Only select repositories** y elige solo tu repositorio del portfolio.
3. *Permissions → Repository permissions → Contents*: **Read and write**. Nada más.
4. Pon una caducidad (por ejemplo 1 año), genera el token y cópialo.

## 4. Activar el editor en tu navegador
1. Abre `https://TU-USUARIO.github.io/portfolio/#editor`.
2. Pega el token. Usuario, repositorio y rama se rellenan solos; revísalos.
3. Pulsa **Validar y guardar**. Aparecerá la barra de edición arriba.
4. Prueba: cambia el nombre en **Ajustes**, pulsa **Guardar cambios**, espera ~1 minuto y recarga la web en una ventana privada.

Cuando quieras empezar con tu contenido, pulsa **Quitar ejemplos** y sube tus imágenes.

## Notas
- Los visitantes no ven nada de edición: solo tu navegador tiene el token.
- Si usas otro dispositivo, repite el paso 4 con un token (puede ser el mismo).
- Para ver cómo lo ve un visitante sin salir: **Ver como visitante**.
- Si el token caduca, crea otro y pégalo en **Ajustes → Cambiar token o repositorio**.
- Para probarlo en tu ordenador necesitas un servidor local (abrir `index.html` con doble clic no carga `datos.json`), por ejemplo `python -m http.server` en la carpeta.
