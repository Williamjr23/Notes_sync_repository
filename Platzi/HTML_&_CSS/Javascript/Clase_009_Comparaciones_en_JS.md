# Comparaciones en JS
### Distintas maneras de comparar variables u objetos en js

Existen cinco tipos de datos que son primitivos:

```js 
Boolean:  // false/true
Null:  // nulo o "vacío"
Undefined: // Cuando una variable es declarada pero aún no tiene un valor asignado 
Number: // 383839
String:  // "esto es una string"```
```



### 1. La primera forma de comparar:

> así como el igual ```=``` sirve para asignar el valor a las variables, el ``` == ``` es nuestra primera forma de comparar en JS 

```js
var x = 4, y = 4
```

> Aquí podemos ver que al comparar ``` x == y ``` nos saldría ```true``` ya que el valor asignado a x es igual al valor que se le es asignado a y, pero sin en vargo el valor de ```x``` está asignado de tipo **numero** y el de ```y``` está asignado como tipo **string**, a pesar de que tengan el mismo valor son diferentes en cuanto al tipo de dato, lo que hace nuestra primera forma de comparar '``` == ```' es pasarnos nuestro dato de tipo **número** a **string** y comparar los resultados ambos en string y por eso la salida o el output de comparar esta operación resultaría en true como podemos ver en el siguiente ejemplo:

```js
x == y 

true
```

>nota: sin embargo, como te podras imaginar esta no es una muy buena practica a menos que la situación lo requiera, aunque en teoría no debería de ser así y se debería trabajar comparando no solo el contenido de los datos si no que también el tipo de dato de cada lado de la comparación, como lo podremos ver en la segunda forma de comparar

### 2. Segunda forma de comparar

En esta segunda forma se hace en lugar de ```==``` se ponen 3 ```===``` y esto lo que hace es que aparte de comparar los datos, tambíen se compara el tipo de dato y es mas preciso, en este caso daría ```false``` devido a que a pesar de que ambos datos son 4 uno está en **string** y el otro está como **numero** como puedes ver esto es mucho mas preciso a la hora de comparar datos, y es mas preferible utilizar esta forma de comparar casi siempre, ya que no tendremos problemas de datos numericos convertidos a strings sin darnos cuenta entre otras cosas es una buena practica.

>nota: utilizar casi siempre que se pueda el triple igual o la segunda forma 

### Comparando objetos:

> Se comparan objetos que aunque sean iguales al interior se llaman diferente y tienen un nombre distinto, definitivamente son variables separadas, en este caso la comparación tanto la primera como la segunda forma no nos daría resultado ```true``` ya que lo que se compara aquí al momento de hablar de objetos, es que literalmente el objeto 1 y el objeto 2 hagan referencia al mismo espacio de memoria (ram) dictada para ese objeto, en el caso de que el objeto 1 hiciera referencia al objeto 1 de la manera siguiente:
```js 
var objeto2 = objeto1
```
 > aquí literalmente se le está diciendo que objeto2 tiene como referencia el valor del objeto1, por lo tanto si se cambia algo en el objeto2 o en el objeto1 se verá afectado el objeto1 y por ende el objeto2, lo que quiere decir que comparte el mismo valor y recurso en memoria del programa, por lo tanto aquí el valor de comparar tanto la forma1 como la forma2 si nos estaría arrojando ```true```

>nota: sin embargo, si se duplica el primer objeto principal dentro de el segundo objeto, sigue sin estar en el mismo espacio de memoria, así que el programa no lo tomará como ígual ya que literalmente al hablar de objetos se refiere a que compartan el mismo dato y ambas dependan de ello.

recordar que se están comparando aquí objetos y no valores primitivos

Entonces como conclución, podemos decir que tenemos que tener en cuanta al usar las comparaciones, con que tipo de dato estamos trabajando, cuales son las buenas practicas mencionadas aquí para trabajar con ese tipo de datos y que los objetos a diferencia de los valores primitivos ya mencionados en la parte de arriba, se manejan de una manera completamente distinta al comparar a pesar de que se comparen con la misma syntax

comparar valores primitivos como numeros o letras no es lo mismo que comparar objetos


