# Git - Guía Rápida

Git es un software de control de versiones diseñado por Linus Torvalds, pensando en la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones cuando éstas tienen un gran número de archivos de código fuente. Al principio, Git se pensó como un motor de bajo nivel sobre el cual otros pudieran escribir la interfaz de usuario o front end como Cogito o StGIT. Sin embargo, Git se ha convertido desde entonces en un sistema de control de versiones con funcionalidad plena. Hay algunos proyectos de mucha relevancia que ya usan Git, en particular, el grupo de programación del núcleo Linux.

### Configuración
* [Linux] - Descarga y configura git en Linux.
* [Windows] - Descarga y configura git en Windows.
* [OSX] -Descarga y configura git en OSX.

### Repositorio Git
Crea un directorio nuevo, ábrelo y ejecuta `git init` para crear un nuevo repositorio de git.

### Clonar Repositorio Remoto
Si utilizas un servidor remoto, ejecuta

```git clone username@host:/path/to/repository```

### Flujo de trabajo
Tu repositorio local esta compuesto por tres "árboles" administrados por git. El primero es tu `Directorio` de trabajo que contiene los archivos, el segundo es el `Index` que actua como una zona intermedia, y el último es el `HEAD` que apunta al último commit realizado.

![local_operations](https://git-scm.com/figures/18333fig0106-tn.png)

### Registro de Cambios
Puedes registrar cambios (añadirlos al Index) usando

`git add <filename>`

`git add .`

Este es el primer paso en el flujo de trabajo básico. 

Para hacer commit a estos cambios usa

`git commit -m "Commit message"`

Ahora el archivo esta incluído en el HEAD, pero aún no en tu repositorio remoto.

### Subir los cambios al repositorio remoto
Tus cambios están ahora en el HEAD de tu copia local. Para enviar estos cambios a tu repositorio remoto ejecuta: 

`git push origin master`

Reemplaza **master** por la rama a la que quieres enviar tus cambios. 

Si no has clonado un repositorio ya existente y quieres conectar tu repositorio local a un repositorio remoto, usa:

`git remote add origin <server>`

Ahora podrás subir tus cambios al repositorio remoto seleccionado.


[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [OSX]: <https://code.google.com/archive/p/git-osx-installer/downloads>
   [Windows]: <https://git-for-windows.github.io/>
   [Linux]: <https://git-scm.com/download/linux/>
