# Funciones como parámetros

>Vamos a hacer que la function saludar acapte un parámetro

Vamos a hacer que cada que una persona salude la function responda el saludo  



>Primero creamos la ```function``` ```responderSaludo``` que toma como parámetros el ```(nombre, ape)
```js
function responderSaludo(nombre, apellido, esDev) {
	console.log(`Buen día ${nombre} ${apellido}`)
	if(esDev) {
	console.log(`Ah mirá, no sabía que eras desarrollador/a`)
	}
}
```
