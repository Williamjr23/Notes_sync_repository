### Cuales son las tareas que se manejan de manera asincrona? 

* Tareas en tiempo futuro
* Interactuar con el DOM (modificar elementos de la pantalla)
* Cambiar clases de CSS
* Mostrar un alert
* Pedidos de datos hacia una API


### Como asignarle un tiempo a los outputs en JS
 
 ```js
 <script>
 	console.log('a')
	setTimeout(function () {
		console.log('b')
	}, 2000)
	console.log('c')
 </script> 
 ```
 >nota: El tiempo se maneja en milisegundos

También lo podemos escribir como arrow function: 

```js
	setTimeout(() => console.log('b'), 2000)
```