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

- `git alias`: No es un comando como tal pero crear alias de comandos extensos nos facilita la tarea de escribirlos, por ejemplo para crear uno es de la siguiente forma: `git config --global alias.nombreAlias "log --graph --decorate --all --oneline"`

- `git diff`: Se utiliza para mostrar las diferencias entre es estado del ultimo archivo y el ultimo commit.

-  `git reset --hard`: Es una instrucción poderosa que se utiliza en Git para restablecer el estado de tu directorio de trabajo (working directory) y el área de preparación (staging area) al estado de un commit específico, descartando todos los cambios que se han hecho desde ese commit.

-  `git reflog`: Muestra un historial de todas tus acciones recientes (como commits, resets, y rebase) y cómo han cambiado los HEADs de las ramas.

- `git tag`: se utiliza en Git para marcar puntos específicos en la historia del repositorio como importantes. Comúnmente, se usa para marcar versiones de lanzamiento de esta forma `git tag v1.0`

- `git branch`: es usado en Git para gestionar las ramas de tu proyecto. Aquí un resumen básico de su funcionalidad:
  - **Listar todas las ramas**: Al ejecutar `git branch` sin argumentos, te muestra una lista de todas las ramas locales en tu repositorio. La rama en la que te encuentras actualmente estará marcada con un asterisco (*).
  - **Crear una nueva rama**: Para crear una nueva rama, usas `git branch <nombre_de_la_rama>`. Esto crea una nueva rama basada en tu posición actual (HEAD), pero no cambia a la nueva rama.
  - **Eliminar una rama**: Para eliminar una rama local, utilizas `git branch -d <nombre_de_la_rama>`. Usa `-D` en lugar de `-d` para forzar la eliminación de una rama que contiene cambios no fusionados.
  - **Renombrar una rama**: Para renombrar la rama actual, puedes usar `git branch -m <nuevo_nombre>`. Para renombrar cualquier rama, usas `git branch -m <nombre_actual> <nuevo_nombre>`.
  - **Ver ramas remotas**: Para ver las ramas en tu repositorio remoto, puedes usar `git branch -r`.

- `git switch`: Sirve para cambiar entre la rama actual a otra rama `git switch otraRama`

- `git merge`: Cuando ejecutas git merge <nombre_de_la_rama>, Git intentará fusionar automáticamente los cambios de <nombre_de_la_rama> en la rama en la que te encuentras actualmente. Si no hay conflictos, Git creará un nuevo "commit de merge" para sellar la fusión.

- `git stash`: Me permite guardar de forma temporal los cambios no compretidos, los que no han sido añadidos con git add y/o git commit.
  - **Listar stashes**: git stash list muestra todos tus stashes guardados.

  - **Aplicar un stash**:
  `git stash pop` aplica el último stash y lo elimina de la lista.
  `git stash apply` aplica el último stash sin eliminarlo de la lista.
  - **Eliminar stashes**:
  `git stash drop <stash@{n}>` elimina un stash específico.
  `git stash clear` elimina todos los stashes.

- `git remote add nombre url`:  Me permite agregar un nuevo repositorio.

- `git fetch`: Se utiliza para actualizar tu repositorio local con los cambios desde un repositorio remoto, pero sin fusionar esos cambios en tus ramas de trabajo actuales

- `git push`: Se utiliza en Git para subir tus cambios locales a un repositorio remoto.

- `git push -u origin main`: Sube los cambios de la rama local main al repositorio remoto origin.
Establece la rama remota main como la rama de seguimiento predeterminada para la rama local main, simplificando futuros git push y git pull en esa rama.

- `git pull`: En Git combina dos acciones en una: primero, actualiza tu repositorio local con los cambios desde un repositorio remoto (haciendo git fetch), y luego, fusiona esos cambios en tu rama de trabajo actual (haciendo git merge).
