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
Simplemente digamos que quieres utilizar la función de: `` 