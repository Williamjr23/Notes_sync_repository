# Estructuras repetitivas for

>Nos va a permitir repetir un codigo cierta cantidar preestablecida de veces 

> Nos va a permitir realizar una tarea de forma repetitiva, y es otra estructura de control

Para esto vamos a utilizar el ```for```seguido de parentesis ```()``` y luego de llaves ```{}```  de la siguiente manera:

```js
for () {

}
```

> Entre las llaves ```{}``` va a ir la parte que queremos que se repita 

> Entre los parentesis ```()``` va a tener 3 partes:
> 1.la parte Inicial
> 2.la parte de la condicion
> 3.la parte del incremento incremento

ahora para la practica de hoy vamos a utilizar un contador, y dentro de un ciclo ```for``` normalmente ese contador se llama ```i``` y quedaría de la siguiente forma

```js 
for (var i = 1;) { 

}
```
> se especifica entonces que la el contador ```for``` va a iniciar desde el numero 1

>nota: con el for lo que inicializamos es el contador que tiene como parametro la variable ```i``` que se iguala a 1 y despues este si se tiene que cerrar terminandose con punto y coma ```;```

>nota: la i es solo el nombre de la variable que se le está indicando, puede significar ```iteration``` ```inicia```, es solo para dar una idea

Luego de la iniciación de el contador anterior, lo que sigue es declarar una condición, y si esta condición se cumple significa que nuestro codigo (Que va a estar especificado dentro de las llaves ```{}```) se va a ejecutar hasta que la condición se deje de cumplir

```js
for(var i = 1; i <= 365;) {

}
```
>nota: la condicion es que el contador "i" sea menor o igual a 365 , para que pase contando y cumpliendo la condición hasta llegar al numero 365 entonces al llegar ahí el codigo dejará de ejecutarse

```js
for(var i = 1; i <= 365; i++) {

}
```
> ```i ++``` al final de la condición, lo que indica es que el contador se incremente cada vez que termina de ejecutar el codgo 

### Generar numeros aleatorios:
 ```js
 var random = Math.random()

if (random < 0.25){
	//aumentaDePeso
} else if (random < 0.5) {
	// adelgazar
	}
} 
```

> La logica de esto nos indica que la variable ```random``` va a ser igual a y estamos llamando a ```math.random() que nos va a generar un numero aleatoreo cada que consultemos esa variable, pero para definir si el numero es mayor a ... aumenta de peso o si es