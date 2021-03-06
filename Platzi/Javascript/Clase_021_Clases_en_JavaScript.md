# Como funcionan las clases en JS?

> Cuando hablamos de objetos en JS estamos hablando de prototipos y no tanto de clases 

>Las clases en JS terminan siendo de cierta manera lo que llamamos prototipos


### Definir un prototipo

> Lo unico que necesitamos hacer es definir una ```function``` por ejemplo en:

```js
function Persona(){
	/// function a ejecutar
}
```

La ```function``` que está definida ahí es la que se va a ejecutar cuando se crea una persona

Por ejemplo sí: 
```js
var william = new Persona()
```

Entonces la función de arriba se va a ejecutar, notemos como tenemos un nuevo argumento aquí que es: ```new``` que es una palabra reservada para el lenguaje, está diseñada y reservada nada más para crear nuevos objetos dado un prototipo, para tenerlo más claro en el código de arriba lo que se hace es crear un nuevo objeto llamado william pero se le asigna el prototipo que se le indique después que en este caso es ```Persona()``` y también implicitamente se va a retornar el nuevo objeto creado sin necesidad de tener un return, como ya se le asigno el prototipo ```Persona()``` entonces ya no tiene que ser retornado explicitamente para saber que sacha pertenece a ```Persona()```

### Parámetros de nuestro prototipo:
Ejemplo: 
> Se envían los datos de el objeto con los parámetros en los paréntesis ```()``` 
```js
var sacha = new Persona('Sacha', 'Lifszyc')
```

> Y anteriormente se definen los parámetros en la functión para que al enviarlos sepa en que lugar de el objeto categorizarlos, en este caso está diciendo que el primer valor del parámetro recibido se tomará como ```nombre``` y el segundo de este mismo como ```apellido```, pero se podrían tomar muchos otros más:
```js
function Persona(nombre, apellido) {
	
}
```
Y para guardarlo dentro de este objeto que se está construyendo en la memoria, podemos hacer referencia a este objeto dentro de esta ```function``` como:
```js
function Persona(nombre, apellido) {
	this.nombre = nombre
	this.apellido = apelldo
}
```
> ```this```, esta etiqueta va a hacer referencia a el objeto que se acaba de construir, mismo objeto del cual estamos definiendo los parámetros que vamos a recibir entre los paréntesis ```()``` de la ```function``` de aquí arriba

> Y también en el caso de el código anterior ```this.nombre``` está diciendo que la variable nombre dentro de el objeto se le va a asignar el = ```nombre``` que estámos recibiendo de nuestro ```new```

> También es importante ver que implicitamente cuando invocamos la functión que define los parámetros de nuestro prototipo con la etiqueta ```new``` como ya lo vimos en la parte de arriba, esta implicitamente te retorna el ```this```


> Nota: Esto es algo que no se tiene que hacer pero se va a explicar para tomarse en cuenta:
> > En caso de no usar la palabra ```new``` se va a construir un objeto y se va a asignar al objeto los atributos  pero es una mala practica 

### Prototype
> Decirle al prototipo que exista una functión

```js
Persona.prototype.saludar = function () {
	console.log(`Hola, me llamo ${this.nombre} ${this.apellido}`)
}
```
> Y esto lo que va a hacer es decir que dentro de el prototipo de persona va a existir el prototipo saludar que va a ser una ```function``` y ahí se definen los parámetros de esta misma por ejemplo en este caso la ```function``` solo imprime un ```console.log```

> **Nota**: Prototype es un constructor de objetos global que está disponible para todos los objetos de JavaScript.