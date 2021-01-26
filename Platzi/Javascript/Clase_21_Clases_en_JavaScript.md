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
