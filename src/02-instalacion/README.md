# Ambiente de desarrollo

## Editor

- [Visual Studio Code](https://code.visualstudio.com/)
  - Extensiones
  - Snippets
- [Atom](https://atom.io/)
- [SublimeText](https://www.sublimetext.com/)

## Navegador / Cliente web

- [Chrome](https://www.google.com/chrome/)
  - Herramientas del desarrollo
    - Elementos
    - Consola
    - Aplicación

## Git/Github

### [Git](https://git-scm.com/)
Git es un sistema de control de versiones distribuido gratuito y de código abierto diseñado para manejar todo, desde proyectos pequeños hasta proyectos muy grandes, con rapidez y eficiencia.

Un repositorio de Git es un almacenamiento virtual de tu proyecto. Te permite guardar versiones del código a las que puedes acceder cuando lo necesites.

#### Flujo de trabajo

Tu repositorio local esta compuesto por tres "árboles" administrados por git. El primero es tu **Directorio** de trabajo que contiene los archivos, el segundo es el **Index** que actua como una zona intermedia, y el último es el **HEAD** que apunta al último commit realizado.

![flujo de trabajo](https://rogerdudler.github.io/git-guide/img/trees.png)

#### Principales comandos

  Crea un repositorio nuevo

  ~~~
  git init
  ~~~

 Para obtener un resumen de qué archivos tienen cambios que se preparan para la próxima confirmación.

  ~~~
  git status
  ~~~

  Puedes registrar cambios, es decir, agregar el contenido al Index. Este es el primer paso en el flujo de trabajo básico.

  ~~~
  git add <filename>
  git add .
  ~~~

  Para hacer commit a estos cambios se usa commit. De esta forma el contenido está incluido en el HEAD.

  ~~~
  git commit -m "Commit message"
  ~~~

  Se pueden visualizar los registro con git log

  ~~~
  git log
  ~~~

### [Github](https://github.com/)

Github es una plataforma de desarrollo colaborativo de software para alojar proyectos usando el sistema de control de versiones Git.

Una vez creado el repositorio en github los cambios se envían a tu repositorio remoto con los siguientes comandos

  ~~~
  git remote add origin https://github.com/USER/REPOSITORIO.git
  git branch -M main
  git push -u origin main
  ~~~

Para enviar los cambios posteriores a tu repositorio remoto solo ejecuta.

  ~~~
  git push
  ~~~

## Servidores gratuitos de prueba

- [Netlify](https://app.netlify.com/)
- [Github Page](https://pages.github.com/)
- [Glitch](https://glitch.com/)
- [Vercel](https://vercel.com/)

## Gestores de paquetes

Un sistema de gestión de paquetes, también conocido como gestor de paquetes, es una colección de herramientas que sirven para automatizar el proceso de instalación, actualización, configuración y eliminación de paquetes de software.

### [NPM](https://www.npmjs.com/)

NPM es parte esencial de [Node.js](https://nodejs.org/es/), responde a las siglas de Node Package Manager o manejador de paquetes de node, es la herramienta por defecto de JavaScript para la tarea de compartir e instalar paquetes.

### [Yarn](https://yarnpkg.com/)

YARN es un gestor dependencias de JavaScript, que está enfocado en la velocidad y la seguridad, y a diferencia de otros gestores como NPM, YARN es muy rápido y muy fácil de usar. Sin embargo, se necesita también Node.js, porque depende de él, ya que utiliza el registro de NPM por defecto.
