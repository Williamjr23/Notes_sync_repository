# ```function``` ```prototype``` a arrow function
### Quien es this?
#### Introducción 
>De cierta manera aquí podríamos decir que ```this``` como anteriormente lo vimos hace referencia a el objeto que se acaba de construir, pero también dentro de una ```arrow function``` funciona de manera diferente apuntando hacia el objeto global que en este caso sería "```window```"

### Que es el objeto window?
>window es el objeto global dentro de el navegador El **objeto window** representa la ventana que contiene un documento DOM; la propiedad document apunta al DOM document cargado en esa ventana. ... Esto significa que el **objeto window** no se comparte entre diferentes pestañas de la misma ventana del navegador.

#### Por que hay que cuidar en donde y como se utiliza el ```this``` para referenciar, para saber siempre hacia donde apunta la ```function```
>Lo que debemos de entender para saber por que nos tira ```undefined``` algunas veces al hacer referencia a un objeto utilizando el ```this``` es por que algunas veces dependiendo de el contexto en que se utilice esta ```function``` va a estar apuntando hacia otro lado.

>Y lo anterior es uno de los errores mas comunes en Js tanto en el backend como en frontend, la función ```this.``` no siempre va a estar referenciando el objeto que esperas que esté referenciando, este es uno de los casos representado al intentar hacer nuestra linea de codigo anterior en una arrow function

```js 
Persona.prototype.soyAlto = function () {
 return this.altura > 1.80
}
```
> Esta es nuestra forma común en la que no tenemos problema referenciando nuestro ```this```

```js
Persona.prototype.soyAlto = () => this.altura > 1.8
```
>En la ```function``` de aquí al usar una arrow function se está referenciando el ```this``` como un objeto global, y como mencionamos anteriormente ```this``` como objeto global hace referencia a window que es el objeto global de el navegador, por lo tanto nunca nos va a funcionar este codigo en forma de arrow function, ya que la ```function``` global no tiene los parametros defindos que estamos pidiendo, pero tampoco dará error ya que la variable this si está siendo referenciada, solo que apunta hacia otro lado


como podemos ver aquí en las arrow functions this no es lo que esperabamos y lo que pasa aquí es que la arrow function asigna esa function pero cambia el ```this``` dentro de la function, lo que hace es que el this lo va a dejar apuntando a el espacio global, y this en el espacio global es window y lo podemos comprobar en la consola de la siguiente manera:

```js
this === window

true
```

>Nota: Esto solo funciona para ```this``` dentro del espacio global ya que ```this``` bien referenciado como lo vimos anteriormente si hace referencia a el objeto que se acaba de construir por ejemplo en el caso de este fragmento de código 
