# GIT y Github  https://github.com/txema-illarramendi
En este documento recogere los pasos que he ido dando con Git y con Github en este trabajo.  

**Listado de comandos usados hasta el momento**

---
1. ``git init``  
nicia el directorio de trabajo donde efectuara el seguimiento
1. ``git add``  
eguido del anombre del rchivo al que se le quiere dar seguimiento o de un punto si se quieren seleccionar todos
1. ``git status -s``  
Muestra el estado de los archivos monitorizados
1. ``git commit -m``  o ``git commit -am``  
pasa los archivos al repositorio local y genera una 'instantanea' o 'foto' de los mismos que almacena con un valor exadecimal.  
Se le suele añadir el modificador -m para añadir un comentario directamente desde la consola sin necesidad de abrir un editor de texto.  
Para hacer un ``commit`` antes hay que haber hecho un add pero podemos hacer directamente el commit sin hacer antes el add añadiendole el modificador -am  
1. ``git remote add origin https://github.com/txema-illarramendi/plaiaundi.git``  
Para indicar la dirección del repositorio remoto
1. ``git branch -M master``  
De esta manera definimos la rama (en este caso la ùnica exixtente)
1. ``git push -u origin master``  
Y con el push de damos un empujon a todo el proyecto al repositorio remoto en la rrama que nos encontremos
1. ``git clone https://github.com/txema-illarramendi/plaiaundi.git``  
Recupera todo el proyecto, por ejemplo para trabajar en una segunda ubicación
1. ``git pull``  
Nos sincroniza con los posibles cambios existentes en el repositorio remoto  
1. ``git log -- oneline``  
Nos muestra los commits de la rama en la que estamos
---
## El archivo .gitignore  
El archivo .gitignore es un archivo sin extensión y como podemos ver por el punto que le precede es un archivo oculto que contendra simplemente texto plano.  
En el indicaremos los nombres de los archivos o directorios a los que no queramos que Git le haga seguimiento.