# Funciones como parámetros

>Vamos a hacer que la function saludar acapte un parámetro

Vamos a hacer que cada que una persona salude y la function responda el saludo 

>Primero creamos la ```function``` ```responderSaludo``` que toma como parámetros el ```(nombre, apellido, esDev)``` y nos retorna un ```console.log()``` y luego decimos que sí es dev ```if(esDev)``` entonces ejecute la siguiente linea de codigo 
```js
function responderSaludo(nombre, apellido, esDev) {
	console.log(`Buen día ${nombre} ${apellido}`)
	if(esDev) {
	console.log(`Ah mirá, no sabía que eras desarrollador/a`)
	}
}
```

Luego a continuación se le va a pasar la ```function``` ```responderSaludo``` a ```saludar()``` como parámetro

```js 
sacha.saludar(responderSaludo)
erika.saludar(responderSaludo)
arturo.saludar(responderSaludo) 
```

Y luego en ambas funciones saludar se le va a poner el parametro el nombre que nosotros queramos y lo que hacemos es que la function sea opcional tal vez la mandan o no se pida el parámetro o no tendrá que seguir funcionando correctamente, ejemplo:
```js 
saludar(fn) {
       var {nombre, apellido} = this
      //  var nombre = this.nombre
      //  var apellido = this.apellido
        console.log(`Hola, me llamo ${nombre} ${apellido} y soy desarrollador`)
        if (fn) {
            fn(nombre, apellido, true)
        }
    }
}
```
> Esta sería el pararmetro que se le da a ```saludar``` que sería ```(fn)``` y con esto ya tenemos la posiblidad de recibir una función dentro de este parametro, en este caso no está definida por eso es ```(fn)``` así que puede recbir cualquer funcion que pongamos como parametro al intentar utilizar la ```funtion``` ```saludar(responderSaludo)``` como por ejemplo ahí que hace que al ejecutarse saludar se ejecute la ```function``` ```(responderSaludo)``` que fue la que se utilizó como parámetro para llamar a esta misma. y de igual manera lo haríamos dentro de la clase Persona 

>nota: La forma de escribir el ```var {nombre, apellido} = this``` como ya lo vimos anteriormente desestructuramos el objeto para poder utilzarlo constantemente dentro de nuestra funcion repetidas veces sin tener que estar accediendo a ```this.``` cada que lo necesitemos, esto nos ahorra espacio

```js
 saludar(fn) {
     var {nombre, apellido} = this
    console.log(`Hola, me llamo ${nombre} ${apellido}`)
    if (fn) {
        fn(nombre, apellido, false)
    }
 }
```
> Aquí podemos ver que tenemos el parametro ```(fn)``` y abajo tenemos asignado un ``` if (fn)``` que lo que va a hacer es tomar valores booleanos para ejecutar lo que esté en la linea de abajo dependiendo si es ```true``` o ```false``` y los valores que soporta son los siguientes:
> 
| nombre    | valor |
| --------- | ----- |
| false     | false |
| 0         | false |
| null      | false |
| " "       | false |
| undefined | false |
| Nan       | false |
> Todos los demás son valores verdaderos, tanto un string con texto o poner directamente ```true``` que es lo más prolijo de hacer a la hora de estar trabajando con estos valores
>> En este caso una ```function``` como valor que existe dentro de un ```if()``` va a ser verdadero y en caso de que no exista va a ser ```undefined``` y como ya mencionamos anteriormente eso se representa como ```false```
>
