# Solución: Git no está instalado

El error que ves (`git : The term 'git' is not recognized`) significa que **Git no está instalado** en tu computadora (o Windows no sabe dónde encontrarlo).

Para subir tu proyecto a GitHub, es obligatorio tener esta herramienta.

## Paso 1: Instalar Git

1.  Ve al sitio oficial: **[https://git-scm.com/download/win](https://git-scm.com/download/win)**
2.  Haz clic en **"Click here to download"** (la versión de 64-bit comenzará a bajar).
3.  Ejecuta el instalador descargado.
4.  Puedes darle a **"Next"** en todas las opciones (la configuración por defecto está bien).
5.  **IMPORTANTE**: Cuando termine, **cierra Trae completamente y vuélvelo a abrir**. Esto es necesario para que el terminal reconozca el nuevo comando.

## Paso 2: Configurar tu usuario (Solo la primera vez)

Una vez reinstalado y reiniciado el terminal, escribe esto (con tus datos reales):

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

## Paso 3: Subir el proyecto

Ahora sí, ejecuta los comandos que fallaron anteriormente:

```bash
git init
git add .
git commit -m "Versión inicial"
git branch -M main
git remote add origin https://github.com/asaltori/menu.git
git push -u origin main
```

## Alternativa: GitHub Desktop

Si prefieres no usar la terminal, puedes descargar **[GitHub Desktop](https://desktop.github.com/)**:

1.  Instálalo e inicia sesión con tu cuenta de GitHub.
2.  Ve a "File" > "Add Local Repository".
3.  Busca y selecciona la carpeta de este proyecto (`c:\Users\asalt\Documents\trae_projects\menu`).
4.  Te preguntará si quieres crear un repositorio ahí. Di que sí.
5.  Haz clic en "Publish repository" y selecciona tu cuenta.
