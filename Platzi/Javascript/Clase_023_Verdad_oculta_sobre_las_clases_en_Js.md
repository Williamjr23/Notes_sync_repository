como hago para que un prototipo herede de otro

js no soporta la herencia por que no soporta las clases, no hay clases, hay prototipos que son objetos que les vamos agregando metodos que reciben funciones, saben quien es this y saben como ejecutarlas, pero no existe un sistema como tal donde se diga que un prototipo va a heredar de otro, lo que si existe es la herencia prototipal

# Herencia prototipal
Como funciona? en js

> crear prototipos hijos a base de un prototipo que va a ser un subtipo de el prototipo principal y lo que podemos decir que este subtipo de va a ver si puede responder a el metodo que queremos llamar, pero si no sabe como responder a ese metodo, lo que hace es buscar en el prototipo padre si lo encuentra, si no lo encuentra entonces va a seguir en la cadena de buscar en el prototipo padre hasta llegar a el prototipo base de todos los objetos que es ```object``` y si object no conoce ese mensaje recien ahí se va a lanzar el error de que no se conoce ese metodo 

Ejemplo practico:

En este caso teníamos un prototipo que era persona que soporta ciertos parametros como valor dentro de este y que tiene funciones que van a hacer que cada persona salude:
```js 
function Persona(nombre, apellido, altura) {
 this.nombre = nombre
 this.apellido = apellido
 this.altura = altura
}

Persona.prototype.saludar = function () {
 console.log(`Hola, me llamo ${this.nombre} ${this.apellido}`)
 }
```
sin embargo lo que queremos hacer ahora es crear un nuevo prototipo "hijo" que soporte las mismas variables (nombre, apellido, altura) p
