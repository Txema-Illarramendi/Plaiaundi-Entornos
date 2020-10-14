# Comandos (MS-DOS), consola CMD  en Windows

| ![Imágen del autor](https://cutt.ly/txema)Txema&nbsp;Illarramendi | Antes de nada, señalar que la verdadera potencia de los siguientes comandos MS-DOS esta en los modificadores y/o parametros que muchos de ellos admiten y que no se muestran aqui.<br>De hecho algunos de ellos solo son funcionales en conjunto con estos añadidos, una buena prueba de esto es el comando que encabeza la lista, `type`, el cual no puede hacer tarea alguna si no le pasamos más información por parametro.<br>Añadir, tambien, de paso que estos no son todos los comandos existentes para la consola de Windows sino una selección de los que me han parecido más significativos. |
|--|---|
<br>

## De gestion de archivos y directorios
- ### **type**
    Crea un archivo pasandole por parametro el nombre y la extensión del mismo, Por ejemplo para crear el archivo de texto nota.txt en nuestro directorio personal pondriamos ``type c/usuarios/usuario/nota.txt``
- ### **>**
    Redirije la salida de los datos si es a un archivo y este ya existe sobreescribira el contenido.
- ### **>>**
    Si queremos añadir texto a continuación del ya existente usaremos el operador >> lo que lo añadira en la linea siguiente de la ultima escrita.
- ### **md o mkdir**
    Crea un directorio, le tendremos que pasar por parametro la ruta y nombre del mismo.
- ### **del o erase**
    Borra archivos, le tendremos que pasar por parametro la ruta, nombre y extensión del mismo.
- ### **rmdir o rd**
    Elimina el directorio que le pasemos por parametro
- ### **copy**
    Copia/renombra el archivo indicado
- ### **.nombreArchivo.txt/directorio**
    Un punto antes de un archivo o directorio le otorgan la condición de oculto
---
## De navegación

- ### **cd**  
    Es el acronimo de change directory y sirve para moverse de directorio
- ### **../**
    Mediante 'cd' y .. subimos al directorio padre
- ### **./**
    Un solo punto simboliza el directorio actual
- ### **cd nombreDirectorio**
    Para 'navegar' a un directorio concreto, incluso si esta en otra unidad/partición, usaremos el comando cd seguido de la dirección/nombre  del directorio
- ### **dir**
    Mediante el comando 'dir' listamos el contenido del direcorio en el que nos encontramos.
---
## Relacionados con la sesión de  usuario, la propia consola o el SO

- ### **ver**
    Indica la versión del SO
- ### **time**
    muestra/establece la hora del reloj del sistema
- ### **systeminfo**
    Muestra información del sistema
- ### **logoff**
    Cierra la sesión actual
- ### **shutdown**
    Apaga el equipo
- ### **cls**
    Vacia 'limpia' la consola de texto
- ### **exit**
    Cierra la consola
---
## Relacionados con la red

- ### **ipconfig**
    Muestra la información de red del equipo
- ### **tracert**
    Muestra los servidores por los que 'viajan' o 'rebotan' los paquetes de una petición web o un ping hasta llegar al servidor de destino
- ### **getmac**
    Devuelve la MAC del equipo
---
## Relacionados  con las unidades de almacenamiento y las particiones

- ### **chkdsk**
    Analiza una unidad o partición 
- ### **format**
    Formatea una unidad o partición con un sistema de archivos
- ### **defrag**
    Desfragmenta el sistema de archivos de una unidad o partición (Actualmente innecesario en las nuevas unidades SSD)
- ### **convert**
    convierte el sistema de archivos de una unidad o partición de FAT32 a NTFS
---
## Un script
- ### **Para terminar esta pequeña 'hoja de apuntes' incluyo el codigo para crear un pequeño script**
    Este scrip nos mostrara el mensaje "Enorabuena has acertado" si le pasas el número 5 como parametro sino no hara nada.  
    Para ello crearemos un archivo con la extensión .bat y dentro escribiremos el siguiente código.  
    Para que funcione deberemos ejecutarlo situandonos con la consola en el directorio donde lo hemos creado o sino añadir dicho directorio al PATH de variables de entorno del sistema

<code>@echo off  
IF [%1]==[0] echo Enorabuena has acertado</code>
