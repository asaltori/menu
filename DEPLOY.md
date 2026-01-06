# Guía de Despliegue (Deployment)

Dado que este entorno local no tiene Node.js/npm instalado, no es posible ejecutar la aplicación localmente (`npm run dev`). Sin embargo, el código está completamente listo para ser desplegado en plataformas de hosting modernas y gratuitas.

## Opción 1: Vercel (Recomendada)

1.  Sube este proyecto a tu repositorio de GitHub, GitLab o Bitbucket.
2.  Ve a [Vercel.com](https://vercel.com) e inicia sesión.
3.  Haz clic en "Add New..." > "Project".
4.  Importa el repositorio que acabas de crear.
5.  Vercel detectará automáticamente que es un proyecto Vite/React.
6.  Haz clic en **Deploy**.
    *   *Nota: He incluido un archivo `vercel.json` para manejar las rutas de la aplicación correctamente.*

## Opción 2: Netlify

1.  Sube este proyecto a tu repositorio git.
2.  Ve a [Netlify.com](https://www.netlify.com).
3.  Haz clic en "Add new site" > "Import an existing project".
4.  Conecta tu proveedor de Git y selecciona el repositorio.
5.  La configuración de build (`npm run build`) y directorio (`dist`) se detectará automáticamente (o leerá el archivo `netlify.toml` que he creado).
6.  Haz clic en **Deploy site**.

## Ejecución Local (si instalas Node.js)

Si deseas ejecutarlo en tu propia máquina más tarde:

1.  Instala [Node.js](https://nodejs.org/).
2.  Abre una terminal en la carpeta del proyecto.
3.  Ejecuta:
    ```bash
    npm install
    npm run dev
    ```
4.  Abre el link que aparece en la terminal.
