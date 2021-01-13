# Arrays
> Estructuras de datos también conocidas como arreglos que nos permiten agrupar cierto tipo de datos dentro de una colección

>iterar: realizar [cierta acción] varias veces

Supongamos que queremos agrupar dentro de una colección a varios objetos que son personas con varos atributos internos cada uno y lo guardaríamos de la siguiente forma:

```js
var personas = [william, Diana, Parsole, Erick, Elsebasduarte]
```
> Para identificar que es un Array se utilzan los corchetes ```[]``` y dentro de estos vamos a ir poniendo cada una de las variables que queremos que contenga nuestro array y se puede componer nuestro array de:
> * Numeros
> * Texto
> * Objetos
> * Funciones
> 
>O podemos incluso hasta mezclar cosas dentro de el mismo array 

Si se quiere acceder al primero de los elementos recordar que se tiene que empezar desde 0 el primer objeto es el objeto numero 0 en este caso sería 
```js 
personas[0] 
```

si quisieramos acceder a la altura se podría poner:
```js
personas[0].altura
```

La propiedad **length** de un objeto que es una instancia de tipo Array establece o devuelve la cantidad de elementos en esa matriz. El valor es un entero sin signo de 32 bits que siempre es numéricamente mayor que el índice más alto en la matriz.