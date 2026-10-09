## 1. Explica la diferencia entre Git y GitHub.

Git es un sistema que permite registrar los cambios de los archivos y llevar un historial de un proyecto. GitHub es una plataforma en internet que permite guardar repositorios y colaborar con otras personas.

## 2. Explica para qué sirve .gitignore.

El archivo .gitignore sirve para indicar a Git qué archivos o carpetas no debe registrar, por ejemplo, archivos temporales, datos privados o la carpeta del entorno virtual.

## 3. Explica por qué .venv no debe almacenarse normalmente en GitHub.

La carpeta .venv contiene el entorno virtual de Python y las librerías instaladas para el proyecto. Normalmente no se sube porque puede ocupar mucho espacio y puede ser diferente según la computadora. En su lugar, se utiliza requirements.txt para instalar las dependencias necesarias.

## 4. Explica para qué sirve requirements.txt.

El archivo requirements.txt contiene una lista de las librerías y sus versiones que necesita el proyecto de Python. Permite instalar esas dependencias en otra computadora mediante el comando pip install -r requirements.txt.

## 5. Explica la diferencia entre Stage, Commit y Push.

Stage es preparar los cambios que se quieren guardar, normalmente usando git add.

Commit es guardar esos cambios preparados en el historial local del repositorio, usando git commit.

Push es enviar los commits del repositorio local al repositorio remoto de GitHub, usando git push.

## 6. Explica por qué un repositorio puede tener varios commits antes de realizar un push.

Un repositorio puede tener varios commits antes de realizar un push porque cada commit guarda un conjunto de cambios en el historial local. Después se pueden enviar todos esos commits juntos a GitHub mediante un push.
"@ | Set-Content .\parte_4\parte_4.md
