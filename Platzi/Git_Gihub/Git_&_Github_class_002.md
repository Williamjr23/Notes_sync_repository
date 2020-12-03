# Git & Github class 002 (Por que usar un sistema de control de varsiones como Git?)

### Por que un sistema de control de versiones?
Por que nos permite mantener el control de los cambios que hacemos en nuestros archivos y trabajar en conjunto con otras personas y **Git** es uno de los sistemas de control de versiones mas famosos creado por linux foundation

### Comandos basicos:
>**Arranca el repositorio:**
>```git terminal
>$ git init
>```
>Empieza en tu biblioteca un repositorio donde se van a ir guardando todos los cambios que se le hagan al archivo

>**Arranca el archivo:**
>```git terminal
>$ git add <nombre_del_archivo.txt>
>```
>El sistema de control de versiones sabe de la existencia del archivo

>**comenta y envía el archivo:**
>```git terminal
>$ git commit -m "version 1"
>```
>Envía los ultimos cambios del archivo a la base del sistema de control de versiones

>**Añade archivos que se hallan cambiado en la carpeta:**
>```
>$ git add .
>```
>Toma archivos que hallan cambiado en la carpeta en la que te encuentres

>**Comenta los cambios y los guarda**
>```
>$ git commit -m "Cambios a v1"
>```
>Guarda el comentario de que se hicieron cambios a la versión 1

>**Ver el estatus de tu git**
>```
>$ git status
>```
>Ver el estatus de tu base de datos (si haces un cambio y no lo haz añadido aquí va a salir)

>**Muestra los cambios**
>```
>$ git show
>```
>Todos los cambios historicos hechos y quien los hizo

>**Historial de un archivo**
>```
>$ git log biografía.txt
>```
>Ver la historia entera de un archivo