# Arrow_functons

### Definir funciones dentro de variables: 
Existe otra manera de escribir funciones que es de la siguiente manera:

1. asignar a una variable una functión:
Ejemplo:
```js
// se puede usar var o const
const esMayorDeEdad = function (persona){
	return persona.edad >= MAYORIA_DE_EDAD
} 
```

Esto es totalmente permitido en JS, asignarle a una ```variable```una ```funcion``` y luego invocarla, simplemente es una funcion y se debe entonces de tratar como tal

>nota: Lo hecho anteriormente se hace para decir que una ```function``` es anonima, osea que no tiene nombre y luego se le asigna a una variable que si tienen un nombre

>nota: Al definir una función dentro de una variable, es preferible utilizar ```const``` en lugar de ```var``` para ayudar a diferenciar que aunque sea una variable se está tratando con una ```function```.

### Arrow Functions (otra forma de definir variables que son funciones)

* Nos ahorramos la palabra ```function``` 
* Y como su nombre lo indica, se utiliza una flecha ```arrow``` que se pone de la siguiente manera: ``` => ```

Y para entenderlo vamos a desglozar como pasamos la forma de escribir la (funcion dentro de la variable) de la que vimos en la parte de arriba, a empezar a pasarla como arrow function con el fin de ahorrar lineas de codigo y que ultimamente se utiliza mas esta forma, el siguiente codigo sería casi exactamente lo mismo que el codigo de arriba solo que está declarado con **Arrow functions** y se escribiria de la siguiente manera:
```js
const esMayorDeEdad = (persona) => {
	return persona.edad >= MAYORIA_DE_EDAD
} 
``` 

>nota: como podemos ver y dijimos arriba, nos ahorramos la palabra ```function```, pero eso no es todo, por que ahora lo iremos desglozando para ver que se ahorrarán 2 lineas completas de el codigo inicial y haciendo lo mismo de manera mas eficiente

### Ahorrando caracteres con Arrow functions:

Aparte de lo que ya vimos anteriormente, podemos obviar algúnos caracteres ya que la forma de escribir arrow functions y a lo hace de manera quizá algo implicita pero si sabes la logica de como funciona, sabrás como utilizarlo a tu favor para ahorrar codigo, en este caso veremos la siguiente linea de codigo y explicaremos que es lo que estamos ahorrano y explicitamente como trabaja esa linea:

Caracteres ahorrados y por qué:

```js
const esMayorDeEdad = persona => {
	return persona.edad >= MAYORIA_DE_EDAD
}
```

* Cuando tenemos un solo paramentro en la function podemos obviar los parentesís ```()```
* Al igual cuando veamos la flecha (arrow) ```=>```podemos obviar que se trata de una ```function``` asi 

```js
const esMayorDeEdad = persona => persona.edad >= MAYORIA_DE_EDAD
```
* Si una ```function``` lo unico que hace es retornar algo, se puede ahorrar y obviar la palabra ```return``` y borrar las llaves ```{}``` que delimitan el cuerpo de la ```function``` e implicitamente van a retornar el valor de lo que siga a continuación del arrow function osea a continuacion de nuestra flecha ```=>``` y va a devolverse (retornarse) el valor de esa comparación 

>nota: y así la ```function``` que teníamos escrita en 3 renglones ahora pasó a solo ser de 1 renglon.

### Desestructurando el parametro de la arrow function:

> Como vimos anteriormente para desestructurar un objeto dentro de el parametro de una función se desestructura dentro de lo que delimita el parametro de la función misma osea en los parentesis ```()```, aquí podemos ver que nos ahorramos los parentesis, pero por eso es importante entender en que contexto y por que es que nos los estamos ahorrando, en este caso es por que tenemos un solo parámetro, pero al desestructurar la arrow functión, el parentesis regresaría y se abririan llaves dentro de este para desestructurar el objeto dentro de los parametros de nuestra función:

Ejemplo: 
```js
const esMayorDeEdad = ({edad}) => edad >= MAYORIA_DE_EDAD
```

De esta manera a la functión se le pasa un objeto que tiene una edad y nos va a retornar si la edad es mayor a la mayoría de edad.

>nota: es un poco complejo de entender esta nomenclatura, pero es recomendado utlizarla

### Negando valores consecutivos dentro de una condicional (If no)

Para denegar un valor es decir que cuando creemos una condicional necesitemos poner "sí esto no pasa entonces..." en lugar de "sí esto pasa entonces"

Se utiliza el: ```!``` para negar dentro de un condicional 

Ejemplo: 

```js
function permitirAcceso(persona) {
 if(!esMayorDeEdad(persona)) {
 console.log('ACCESO DENEGADO')
 } else { 
 console.log('ACCESO CONCEDIDO')
 }
}
```
>nota: y recuerda que este codigo de arriba también se puede escribir como arrow function u.u 

tarea:
Escribir la function es menor de edad como arrow function y que retorne la negacion de la llamada a es mayor de edad 