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

Entonces la función de arriba se va a ejecutar, notemos como tenemos un nuevo argumento aquí que es: ```new```