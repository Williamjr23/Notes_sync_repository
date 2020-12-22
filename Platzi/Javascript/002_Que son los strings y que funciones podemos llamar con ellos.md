Nueva forma de concatenar strings un poco más nueva:

Interpolación de texto

se utiliza la comilla invertida 

nos permite interpolar variables

aprendimos a usar las funciones mas utilizadas de los strings,
vimos como pasar un string a min a mayus, como saber cuantas letras tiene un string, como acceder a una letra en particular, y como acceder a un substring dentro de un string

Archivos utilizados en: Clase2.js

Funciones que trabajen con decimales, a manera de almacenar decimales no es tan precisa

Para arreglar ese problema se puede hacer 

para solo un decimal mutiplicar antes * 100, luego hacer la operacion y volver a dividir entre 100

si es una operación mas precisa, utilizar 

```javascript 
var total = Math.round(precioDeVino * 100 * 3) / 100
```

Y de esta manera se hace mas preciso el calculo con decimales, sin importar la cantidad de decimales en la cifra original

y para hacer que salga el cero despues de el decimal se declara que se tengan en cuenta el numero de decimales que se quieren mostrar despues del punto, en este caso son 2 Ejemplo:

```js
var totalStr = total.toFixed(2)
```
>nota: Al hacer lo anterior, el resultado de este queda como un string, y para volverlo a pasar a numero hacemos lo siguiente:

```js
var total12 = parseFloat()
```
> Significa transformar o leer de un string a un decimal