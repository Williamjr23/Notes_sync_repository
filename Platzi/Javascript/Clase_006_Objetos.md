# Objetos

Añadir variables a cada rato no es la mejor opción, por eso vamos a empezar a trabajar con objetos, y este reune ciertas características en común, como si fuerán características como en lugar de:

```js
var nombre = 'william'
var apellido = 'Castillo'
```

se podría delimitar el objeto de la siguiente manera:

```js
var william = {
	nombre: 'William',
	apellido: 'Castillo',
	edad: 28
}

var dario = { 
	nombre: 'Dario'
	apellido: 'Susnisky'
	edad: 27
}

```
>se agregan los atributos dentro de el objeto y se separan por comas "```,```"
>Así vemos que un objeto no es nada más que clave y valor.
>Lo de la izquierda es la clave o key, y lo de la derecha es el valor que se le otorga.
>los valores pueden ser strings, numeros, funciones, booleanas... entre otras.

### Acceder a las variables dentro de el objeto
Simplemente digamos que quieres utilizar la función de: ``` imprimirNombreEnMayusculas(nombre)```, la cual es:

```js
function imprimrNombreEnMayusculas(nombre) { 
	nombre = nombre.toUpperCase()
		console.log(nombre)
} 
```
La cual indica que se va a imprimir en la consola el ```nombre``` especficado en la variable local de la función, toma en cuenta que nombre dentro de esta, se refere al nombre dentro de la varable especifcada, con la tarea de imprimr el output con mayusculas y esto se accede:

```js
imprimirNombreEnMayusculas(william.nombre)
imprimirNombreEnMayusculas(dario.nombre) 
```

En el cual indícas, que se use la función anteriormente especificada para imprimir el nombre en mayusculas, en otro caso podría ser cualquer función, y especifcamos en los parametros de nuestra función, que dentro de el objeto ```william```se busque la variable ```nombre``` y el output se pase a mayusculas todo, así mismo dentro de el mismo objeto (willam) podríamos acceder a otras variables como apelldo, o edad.

Otra forma de escrbir esto mismo podría ser:
```js 
function imprimrNombreEnMayusculas(persona) {
	console.log(persona.nombre.toUpperCasse())
}

imprimirNombreEnMayusculas(william)
imprimirNombreEnMayusculas(dario)  
```
> Toma en cuenta que la forma de escribir este codigo, a pesar de que el output sea el mismo, va a depender de nuestras necesidades, o de que tan general, especfico o si queremos re utilzar alguna parte de nuestro codigo.

Y una de las formas en teoría mas descriptivas a simple vista al estár trabajando con el codigo podría ser una como la siguiente, en esta, como lo que nos interesa es la variable nombre dentro de el objeto, lo que podemos hacer, es desglosar el objeto en los parametros y funciona en lugar de escribir dentro de el parentesis de la funcion que son los parametros de la misma pondríamos llaves: ```{ nombre }```

Ejemplo:

```js
function imprimrNombreEnMayusculas({nombre}) {
	console.log(nombre.toUpperCasse())
}

imprimirNombreEnMayusculas(william)
imprimirNombreEnMayusculas(dario) 
```

Definir un objeto dentro de llamar a una función, se define el objeto dentro de la llamada de la función:
```js 
imprimirNombreEnMayusculas({ nombre: 'Pepito' }) 
```

Al igual que si quisieramos definir:

```js
imprimirNombreEnMayusculas({ apellido: 'Gomez' }) 
```
no funcionaría, ya que no tenemos dentro de los parámetros, definido que utilize la variable apellido, así que aunque le demos que apellido es igual a 'Gomez' no va a funcionar ya que dentro de nuestra función, no hay nada establecido a hacer con el apellido.

Detalles de la clase:

* Declarar objetos
* Definir atributos de los objetos
* Asignar valores a cada uno de ellos
* Pasar objetos como parametros hacia las funciones