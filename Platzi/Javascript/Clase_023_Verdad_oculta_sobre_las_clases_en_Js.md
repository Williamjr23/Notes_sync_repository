como hago para que un prototipo herede de otro

js no soporta la herencia por que no soporta las clases, no hay clases, hay prototipos que son objetos que les vamos agregando metodos que reciben funciones, saben quien es this y saben como ejecutarlas, pero no existe un sistema como tal donde se diga que un prototipo va a heredar de otro, lo que si existe es la herencia prototipal

# Herencia prototipal
Como funciona? en js

> crear prototipos hijos a base de un prototipo que va a ser un subtipo de el prototipo principal y lo que podemos decir que este subtipo de va a ver si puede responder a el metodo que queremos llamar, pero si no sabe como responder a ese metodo, lo que hace es buscar en el prototipo padre si lo encuentra, si no lo encuentra entonces va a seguir en la cadena de buscar en el prototipo padre hasta llegar a el prototipo base de todos los objetos que es ```object``` y si object no conoce ese mensaje recien ahí se va a lanzar el error de que no se conoce ese metodo 

Ejemplo practico:

En este caso teníamos un prototipo que era persona que soporta ciertos parametros como valor dentro de este y que tiene funciones que van a hacer que cada persona salude:
```js 
function Persona(nombre, apellido,) {
 this.nombre = nombre
 this.apellido = apellido
}

Persona.prototype.saludar = function () {
 console.log(`Hola, me llamo ${this.nombre} ${this.apellido}`)
 }
```
sin embargo lo que queremos hacer ahora es crear un nuevo prototipo "hijo" que soporte las mismas variables (nombre, apellido,) pero en lugar de ser personas se van a referenciar como Desarrollador
```js 
function Desarrollador(nombre, apellido) {
 this.nombre = nombre
 this.apellido = apellido
} 

Desarrollador.prototype.saludar = function () {
	console.log(`Hola, me llamo ${this.nombre} ${this.apellido} y soy desarrollador`)
}
```
primero dejar en claro que un prototipo es la forma de añadir una function a nuestro objeto que ya ejerce como una function y por eso es que le conocemos como prototipo. ahoria si como podemos ver ambos prototipos responden al mismo nombre de ```saludar``` la diferencia entonces está en qué valor se va a pisar primero e indicarle en que parametros de qué objetos tiene que buscar nuestro prototipo, en pocas palabras debemos definir que objeto va a heredar características de que otro objeto, tales como los prototipos, así cuando se ejecuta el codigo y se añaden valores nuevos a cada objeto, y luego queramos utilizar esa información para generar el saludo por ejemplo, si definimos a una persona como desarrollador ejecutará el saludo de el desarrollador y si definimos a otra como solo persona ejecutará el saludo de persona, sin embargo tenemos funciones extra aquí que son las que nos interesa, saber que función se tiene que pisar encima de cual para saber como escribir nuestro codigo, en este caso necesitamos que la función de desarrollador e