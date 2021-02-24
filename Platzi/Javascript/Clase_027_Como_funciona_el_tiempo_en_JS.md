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

>En principio, cualquier tarea que se haya delegado al navegador a través de un callback, deberá esperar hasta que todas las instrucciones del programa principal se hayan ejecutado. Por esta razón el tiempo de espera definido en funciones como setTimeout, no garantizan que el callback se ejecute en ese tiempo exactamente, sino en cualquier momento a partir de allí, sólo cuando la cola de tareas se haya vaciado.
