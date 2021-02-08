# Funciones como parámetros

>Vamos a hacer que la function saludar acapte un parámetro

Vamos a hacer que cada que una persona salude la function responda el saludo  



>Primero creamos la ```function``` ```responderSaludo``` que toma como parámetros el ```(nombre, apellido, esDev)``` y nos retorna un ```console.log()``` y luego decimos que sí es dev ```if(esDev)``` entonces ejecute la siguiente linea de codigo 
```js
function responderSaludo(nombre, apellido, esDev) {
	console.log(`Buen día ${nombre} ${apellido}`)
	if(esDev) {
	console.log(`Ah mirá, no sabía que eras desarrollador/a`)
	}
}
```

