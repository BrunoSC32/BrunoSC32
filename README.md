### Hi there 👋

# Git y GitHub

## Apuntes que tomé del curso "Curso de GIT y GITHUB desde CERO para PRINCIPIANTES" de "MoureDev by Brais Moure"
[Curso de Git y GitHub](https://www.youtube.com/watch?v=3GymExBkKjE)

### Comandos:

- `git init`: Cuando ejecutas este comando en una carpeta, Git comienza a vigilar esa carpeta, permitiéndote empezar a guardar versiones de tu proyecto en el tiempo (commits).

- `git add .`: Seleccionas los archivos que has cambiado y les dices a Git que los prepare para el próximo registro, utiliza punto (.) para seleccionar todos los archivos sino sustituye el punto por el archivo en específico que quieres añadir.

- `git commit -m "mensaje"`: Haces oficial que los cambios que marcaste con `git add` son importantes y les pones un mensaje para recordar qué hiciste exactamente en ese momento.

- `git log`: Te mostrará un resumen de todas las entradas anteriores (commits), quién las hizo, cuándo y qué decían.

- `git status`: Te muestra qué cambios tienes listos para ser guardados (staged), cuáles no y si hay archivos que Git no está siguiendo.

- `git checkout nombreFichero`: Esto restaurará el archivo `nombreFichero` a su último estado comiteado, eliminando cualquier cambio que hayas hecho desde entonces.

- `git reset`: Poner solo el comando `git reset` te mostrará los ficheros modificados comparándolo desde el último commit.
