# Clases o Prototipos?
> Por mas que se utilice la plabra class que hace referencia a clases, se va a seguir trabajando con prototipos, lo que vimos en la clas anterior fué la forma de generar herencia antes de el estandar EcmaScript 15, y ahora se utiliza una forma mas sencilla de trabajar con la herenia que es lo que veremos el día de hoy pero sin perder las bases de la clase anterior

# Construyendo clases:
Ejemplo:
```js
class Persona {
 constructor(nombre, apellido, altura) {
 this.nombre = nombre
 this.apellido = apellido
 this.altura = altura
	}
	
	 saludar() {
 console.log(`Hola, me llamo ${this.nombre} ${this.apellido}`)
 }
 
  soyAlto() {
 return this.altura > 1.8
 }
}
```
> Aquí declaramos que va a existir la ```class``` (clase) ```persona``` y que va a tener un metodo llamado ```constructor``` que es el que se va a ejecutar cuando creemos objetos de esta clase 
> Además le agregamos el saludar de antes sin necesidad de la palabra function y también el metodo ```soyAlto```


# Como logramos que una clase herede de otra?
Ejemplo:
```js
class Desarrollador extends Persona {
 constructor(nombre, apellido, altura) {
 	super(nombre, apellido, altura)
 this.nombre = nombre
 this.apellido = apellido
 this.altura = altura
 }

 saludar(){
 console.log(`Hola, me llamo ${this.nombre} ${this.apellido} y soy desarrollador`)
 }
}
```

> Aquí creamos la ```class``` ```Desarrollador``` y le decimos antes de las llaves la parte de la herencia, y lo que se llama "herencia" aquí le llamaremos extención ```extends``` así que diremos que esta clase extiende de ```persona```

> No se puede utilizar ```this.``` dentro de el ```extends``` (constructor) hasta que no hallamos llamado a el constructor de la clase padre, y para eso utilizamos la palabra ```super()``` y le pasamos los parametros