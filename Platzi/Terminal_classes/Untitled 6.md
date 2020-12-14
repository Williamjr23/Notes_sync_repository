# Terminal class 007 (Procesamiento de datos)

## Flujos estandar:

Linux/Unix cada nuevo proceso generado, cada nueva aplicación ejecutada es inicializada con tres canales de datos, canales conocidos cómo streams (corrientes).

- **Standar Input**
>Es la entrada de datos de nuestro programa, los datos serán ingresados durante la ejecución del mismo y se harán mediante teclado.
- **Standar Output**
>El programa colocará todos los mensajes que necesita que el usuario visualice. Estos mensajes no deben de considerarse advertencias o errores.
- **Standar Error**
>El programa colocará todos los mensajes de advertencias y errores que puedan sucitarse durante la ejecución del mismo.

## Trabajar con inputs y outputs

Sintaxis:
>```terminal
>history > nombre_del_archivo.txt
>```
>Con el signo "mayor que", crearemos el archivo si este no existe e indicamos que coloque el output del programa en el.
>
>*nota: Sí el archivo ya existe, el contenido será reemplazado por el output del programa.*

Si en lugar de :
```
>
```
ponemos:
```
>>
```
Ejemplo:
```terminal
history >> nombre_del_archivo.txt
```
>Esa instrucción hará que el output sea agregado al final del archivo, sin reemplazar nada.
>
>*nota: El contenido ya no será remplazado si no agregado.*


## Pipes

El simbolo pipe:
```terminal
|
```
Lo que hace es tomar el output de un "proceso" y pasarlo directamente como input a un "proceso" siguiente.

>Ejemplo:
>```terminal
>history | more
>```
>En este casto el:
>```terminal
>more
>```
>Lo que hace es mostrar un resultado largo dividido en varias iteraciones para mas facil lectura (muestra el texto por bloques).

>**Un buen uso practico:**
>```terminal
>history | grep "mkdir"
>```
>En este caso el comando indica que se invoque el historial y con pipe pase directamente al siguiente proceso que sería "grep" y como ya vimos anteriormente en este caso serviría para buscar información directamente dentro de el historial sin siquiera tener que abrirlo.
>
>*nota: En este caso estaría buscando en el historial todos los comandos que hallamos introducido con "mkdir" hasta el momento.*

>**Otro uso practico:**
>```terminal
>cat archivo.txt | wc -l
>```
>En este caso el comando:
>```terminal
>cat archivo.txt
>```
>como ya lo vimos anteriormente este comando concatena el "archivo.txt" pero en este caso el output no va a ser nuestra pantalla ya que con:
>```terminal
>| wc -l
>```
>le indicamos a la terminal que con el output de nuestro archivo directamente realize un input en este caso es:
>```terminal
>wc 
>```
>Que significa: (word count) y como su nombre lo dice por si solo cuenta en orden las:
>**lineas, palabras y caracteres**
>
>Por ultimo:
>```terminal
>-l
>```
>Es parte del repertorio de añadidos a wc y este nos muestra solo el numero de lineas.
>
>