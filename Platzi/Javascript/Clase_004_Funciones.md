# Funciones

> Rapidamente las funciones son pedasos de codigo reutilizables, crearemos nuestras propias funciones para después utilizarlas 

Para definir una función, se va a utilizar la palabra: ```function```la cual está reservada unicamente para esto y no puedes tener variables llamadas con este nombre.

Se pone function y luego el nombre de la funcion, luego los parentesis y adentro de se definiran los parametros, y para delimitar el cuerpo de la funcion se van a utilizar las llaves: ```{}```

Ejemplo:

```js
function imprimirEdad() {
	console.log('${nombre} tiene ${edad} años')
}

imprimirEdad()
```

### Parametros
Se le indíca a la funcion que variables va a recibir, por ejemplo:

```js
var nombre = 'william', edad = 28


function imprimirEdad(n, e) {
	console.log('${nombre} tiene ${edad} años')
}

imprimirEdad(nombre, edad)
```

Así sei ip