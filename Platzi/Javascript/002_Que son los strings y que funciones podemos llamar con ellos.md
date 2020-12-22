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

```
var total = Math.round(precioDeVino * 100 * 3)
```