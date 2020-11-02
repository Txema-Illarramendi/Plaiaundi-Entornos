# Introducción a Git
![Git logo](img/git.png)
## **Pregunta 1:** ¿Qué es Git?  
Git es un sistema de control de versiones pensado para tener un control sobre los cambios y ramificaciones del software al trabajar en un equipo de desarrolladores o en proyectos complejos
## **Pregunta 2:** ¿Cuál es la diferencia entre un "repositorio simple" y un "directorio de trabajo"?  
Un repositorio de trabajo creado con <code>git init</code> es para… **trabajar**  
Un repositorio desnudo creado con <code>git init --bare</code> es para ... **compartir**.  

Los repositorios creados con <code>git init --bare</code> se denominan repos desnudos. Están estructurados de manera un poco diferente a los directorios de trabajo. En primer lugar, no contienen una copia funcional o extraída de sus archivos fuente.
 
Los desarrolladores clonarán el repositorio descubierto compartido, realizarán cambios localmente en sus copias de trabajo del repositorio y luego volverán al repositorio compartido para que sus cambios estén disponibles para otros usuarios.  

Por ejemplo, si un desarrollador está colaborando con un equipo de desarrollo, y necesita un lugar donde compartir los cambios realizados sobre un repositorio, será necesario crear un repositorio <code>bare</code> en un servidor centralizado donde todos los desarrolladores puedan enviar sus cambios (git push).
## **Pregunta 3:** ¿Cuál es la diferencia entre una "bifurcación" y una "rama"?  
Una bifurcación es una diferencia dentro de una rama.
Una rama, en cambio, tiene su propio nombre, esta monitorizada por Git de manera autonoma
## **Pregunta 4:** Has creado una confirmación y la has enviado, ahora es pública.   Sin embargo, has notado que todavía hay cosas que deben cambiarse. ¿Puedes hacerlo en la etapa de confirmación? y si es así, ¿Cómo?  
Si, aún pueden realizarse cambios, incluso después del commit. La forma de hacerlo es emitiendo uno de los comandos git llamado revert.   
El comando actuará como un "parche" para la confirmación que debe cambiarse. De esta manera, incluso si te has olvidado de cambiar algo antes de implementar la confirmación en la versión en vivo, aun puedes alterar y arreglar las cosas después.
## **Pregunta 5:** ¿Qué es "cherry-picking"?
Hace referencia a cuando decides elegir algún tipo de confirmación de una rama basada en Git y luego aplicar sus características a otra rama. Ahora, te preguntaras, ¿Por que esto se denomina "cherry-picking"? Sencillo, la mayoría de los demás comandos Git que se basan en transferencias de confirmación están diseñados para copiar simultáneamente múltiples confirmaciones. Con cherry-picking, podrás elegir una confirmación y aplicarla en otra rama.  
## **Pregunta 6:** ¿Qué es un "stash"?  
Sirve para guardar el area de trabajo actual en una 'pila' provisional para poder luego recuperarla y seguir trabajando, dejando asi vacia/libre el workspace.  
Muy util por ejemplo si, de repente, tienes que dejar apartado el trabajo que tienes entre manos para ponerte con otro que tiene urgencia.  
Necesitas que no se pierdan los avances que llevas hechos en el workspace pero el trabajo tampoco esta terminado como para hacer un ``commit``  
## **Pregunta 7:** ¿Cuál es la diferencia entre commit y push en GIT?  
En términos muy básicos push manda los cambios a tu repositorio remoto, mientras commit lo hace al repositorio local.  
![logo](img/map_git.png) 
## **Pregunta 8:** ¿Cuál es el lenguaje utilizado en Git?
 Git utiliza el lenguaje "C".  
 "C" permite que Git sea excepcionalmente rápido, algo que sería muy difícil de lograr con algunos de los lenguajes de programación más avanzados.
## **Pregunta 9:** ¿Qué es una "solicitud de extracción"?
Cuando tomas un repositorio y creas tu propia rama después de esto, realizas algunos cambios y quieres fusionar dicha rama al proyecto principal.
## **Pregunta 10:** ¿Cómo se utilizan los tags en Git?  
Un commit puede existir (o no) en tu repositorio local o en cualquiera de tus repositorios remotos.
Dicho esto, la única limitación es que tienes es no poder asociar un tag a un commit que no existe.

Puedes hacer commit, crear el tag, hacer push del commit y hacer push del tag. Puedes hacer commit, hacer push del commit, crear el tag y hacer push del tag.

No puedes crear el tag de un commit que no existe. Puedes hacer un commit y un tag, pero si quieres subir el tag deberán antes hacer push del commit pues de lo contrario no habría referencia en el repositorio remoto hacia un commit que no ha sido subido.