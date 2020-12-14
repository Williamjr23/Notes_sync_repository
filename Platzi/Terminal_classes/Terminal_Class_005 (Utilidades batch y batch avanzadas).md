# Utilidades batch y batch avanzadas

Utilidades batch o procesamiento por lotes:

>Programas que procesan texto y emiten el resultado

Utilidades batch

- Grep: Búsqueda por expresiones regulares
Syntax
```Terminal
grep <texto a buscar> <en que archivo se va a buscar.extencion del archivo>
```
Ejemplo:
```terminal
grep Hola HolaMundo.txt 
```
>Función:
>
>Se usa para buscar un texto especifico sobre un archivo de texto plano
>```
>grep
>```
>

Ejemplo:
```terminal
grep -i hola HolaMundo.txt 
```
>Función:
>
>Hace que no importe si esta en mayusculas o minusculas
>```
>-i 
>```

Ejemplo:
```terminal 
grep -i "mundo$" HolaMundo.txt
```

>Función:
>
>El "Hola$" busca solo si la palabra esta al final de la linea
>```
>"Palabra_a_buscar$"
>```
>
>*Nota: Recuerda que si la linea termina con parentesis o coma, etc... se tiene que especificar si no no servirá este comando
>
Ejemplo:
>```
>grep "^Hola" HolaMundo.txt  
>```
>Función:
>El "^Palabra_a_buscar" busca solo si la palabra está al principio de la linea

- Sed: (string editor) Tratamiento de flujos de caracteres 

>Nota: El comando "sed" no modifica el archivo, crea un nuevo flujo a partir de el ya existente pero con los nuevos datos

Ejemplos:
```terminal
sed 's/Mundo/Hola/' HolaMundo.txt
```

>Función:
>
>Puede realizar muchas funciones en archivos como buscar, encontrar y reemplazar, insertar o eliminar.El uso más común del comando es para sustitución o para buscar y reemplazar.
>
>```
>sed
>```
>
>*Nota: Al usar "sed" puede editar archivos incluso sin abrirlos, que es una forma mucho más rápida de encontrar y reemplazar algo en un archivo, que primero abrir ese archivo en un editor y luego cambiarlo.*
>
>
>Se utiliza para indicar que se va a sustituir el elemento
>```terminal
>'s/
>```
>El primero es el elemento que se va a cambiar y el segundo el que lo remplazaría
>```terminal    
>/Mundo/Hola'
>```
>Es el archivo al que se indica que se tiene que ejecutar el comando
>
>```terminal
>HolaMundo.txt 
>```

*Este es un [link](https://likegeeks.com/es/sed-de-linux/) de mas funciones sobre el comando:*
```terminal
sed
```
- Awk: tratamiento de texto delimitado

Es parecido a "sed" se puede utilizar para seleccionar en el texto por columnas o lugares especificos e incluso se pueden realizar operaciones con los elementos seleccionados, utiliza un lenguaje de scripting está potente para sacar calculos de tus datos sin tener que abrir o modificar el texto u.u (lo veré a fondo mas adelante)


༼ つ 7 u 7 ༽つ FIN
