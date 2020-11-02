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
Hace referencia a cuando decides elegir algún tipo de confirmación de una rama basada en Git y luego aplicar sus características a otra rama. Ahora, te preguntaras, ¿Por que esto se denomina "cherry- picking"? Sencillo, la mayoría de los demás comandos Git que se basan en transferencias de confirmación están diseñados para copiar simultáneamente múltiples confirmaciones. Con cherry-picking, podrás elegir una confirmación y aplicarla en otra rama.  
## **Pregunta 6:** ¿Qué es un "stash"?  

## **Pregunta 7:** ¿Cómo resuelves "conflictos " en Git?
## **Pregunta 8:** ¿Cuál es el lenguaje utilizado en Git?
## **Pregunta 9:** ¿Qué es una "solicitud de extracción"?
## **Pregunta 10:** ¿Cuál es la manera más eficiente de encontrar una mala confirmación?
# Preguntas de entrevista Git - Avanzadas
## **Pregunta 1:** ¿Qué es un "encabezado"?  
## **Pregunta 2:** ¿Para qué se utiliza el comando "Git CONFIG"?  
## **Pregunta 3:** ¿Se pueden arreglar las confirmaciones rotas?  
## **Pregunta 4:** ¿Cuál es la diferencia entre "obtener" y "extraer"?  
# Conclusiones