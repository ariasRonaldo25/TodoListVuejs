# TodoListVuejs
Ejemplo sencillo de una to do list usando el framework para frontend vuejs

Es una app de gestión de tareas, una herramienta de productividad muy típica.

# Instalación.
Para ejecutar el proyecto localmente:

1.Es necesario instalar todas las dependencias a través del siguiente comando:

npm install.

2.Luego de realizar la anterior instalación de dependencias, utiliza el siguiente comando para compilar y ejecutar el proyecto.

npm run serve.

Abra su navegador en localhost:8080

# Deploy.
1.Primero debes crear una nueva rama a la que llamaremos gh-pages:
git checkout -b gh-pages

2.A continuación debes crear el archivo vue.config.js en el directorio raíz del proyecto, de modo que podamos establecer las opciones de compilación de Vue. Debes establecer el directorio público en el que estarán los archivos del proyecto. El directorio, una vez esté el proyecto en GitHub Pages, tendrá el mismo nombre que el repositorio asociado, por lo que debes agregar lo siguiente, reemplazando nombre-repositorio por el nombre de tu repositorio en GitHub:

module.exports = {
  publicPath: '/nombre-repositorio',
}

3.Si deseas desplegar el proyecto es necesario realizar un build del proyecto para generar el directorio /dist.

npm run build.

4.Ahora debes agregar el directorio /dist al repositorio ejecutando este comando:

git add dist.

5.Luego haz un commit de los cambios realizados:
git commit -m "gh-pages commit"

6.Finalmente haz un push de la rama gh-pages a GitHub, agregando el prefijo dist:
git subtree push --prefix dist origin gh-pages

Aplicación desplegada: https://ariasronaldo25.github.io/TodoListVuejs/

