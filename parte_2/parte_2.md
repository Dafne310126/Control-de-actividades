Fork: crea una copia del repositorio original dentro de tu propia cuenta de GitHub.

Clone: descarga esa copia a tu computadora para trabajar con ella desde Visual Studio Code.

Branch: crea una rama nueva para trabajar sin afectar directamente la rama principal.

Modificar archivos: realiza los cambios necesarios en el código o los documentos.

Commit: registra los cambios realizados con un mensaje descriptivo.

Push: sube los commits de tu computadora a tu repositorio en GitHub.

Pull Request: solicita que los cambios se revisen para incorporarlos al repositorio original.

Review: el propietario u otros colaboradores revisan los cambios y pueden aprobarlos o pedir correcciones.

Merge: integra los cambios aprobados en la rama de destino del repositorio original.


Fork y Clone

La afirmación es incorrecta, porque Clone no crea una copia dentro de mi cuenta de GitHub.

Fork crea una copia del repositorio en mi cuenta de GitHub, mientras que Clone descarga el proyecto a mi computadora para poder trabajar en él desde Visual Studio Code.

Pull Request

¿Los cambios ya forman parte del repositorio original?

No. Aunque hayas realizado Fork, Clone, Branch, Modificar archivos, Commit y Push, los cambios solamente están en tu propia copia del repositorio en GitHub.

¿Qué debe ocurrir para incorporarlos?

Debes crear un Pull Request para proponer los cambios. El propietario revisa el contenido y, si está de acuerdo, los aprueba y realiza el Merge. Así los cambios se incorporan al repositorio original.

Request Changes

Si el propietario selecciona Request Changes, significa que debo corregir algunos detalles de mi trabajo.

Primero reviso sus comentarios, modifico los archivos, hago un nuevo Commit y después ejecuto Push para subir las correcciones.

No necesito crear otro Pull Request, ya que el que está abierto se actualiza automáticamente cuando subo los cambios desde la misma rama.

Merge y repositorio local

Esto sucede porque el Merge realizado en GitHub no actualiza automáticamente los archivos que el propietario tiene guardados en su computadora.

Para obtener los cambios, debe abrir la terminal en la carpeta del proyecto y ejecutar:

git pull origin main

Este comando descarga e integra los cambios de la rama main del repositorio remoto en la rama local actual.

Sync Fork

Utilizaría la opción Sync fork de GitHub para actualizar mi copia con los cambios que se hicieron en el repositorio original.

Esta herramienta actualiza mi Fork en GitHub. En cambio, git pull descarga los cambios de un repositorio remoto y los integra en mi repositorio local.

Registrar el cambio en un cuarto commit y subirlo a GitHub

Primero guardo el archivo con las respuestas en Visual Studio Code. Después abro la terminal y compruebo los commits anteriores:

git log --oneline -4

Si ya tengo tres commits, agrego el archivo y creo el cuarto:

git add nombre-del-archivo
git commit -m "Agrega respuestas de Git y GitHub"

Por último, subo los cambios a GitHub, usando el nombre de mi rama:

git push origin main

Para comprobar que todo quedó guardado, ejecuto:

git status

Si no aparecen cambios pendientes, significa que mi directorio de trabajo está limpio.
