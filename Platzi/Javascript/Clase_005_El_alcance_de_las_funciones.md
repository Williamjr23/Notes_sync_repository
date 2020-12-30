# Alcance de las funciones:
> Es decir a que variables pueden acceder, y que valores pueden tener esas variables a la hora de invocar esa funcion

  
```
function imprimirNombreEnMayusculas({nombre}) { 

 console.log(nombre.toUpperCase())

}
```
> como podrás ver en la función anterior, expresamente lo que hace es imprimir el string de un nombre para que su output sea el nombre en mayusculas.

A que variables pueden acceder y que valores van a tener esas variables

### Variables globales

Cuando tenemos una variable global?

> Si una variable no está definida dentro de una funcion, se dice que es de alcance global y eso significa que se puede acceder desde cualquier function

> nota: El objeto global en html es la ventana 

Esto no siempre es una buena practica (El hacer muchas variables globales), ya que tiene un sideeffect que modifica la variable global y normalmente queremos poder seguir accediendo a ella sin que esté modificada, y esto lo hacemos de la siguiente manera:

se le agrega un parametro a la función, en este caso es ```(n)``` 

```js
var nombre = 'william'

function imprimirNombreEnMayusculas(n) {
	n = n.toUpperCase()
}
```
/ terminar apunte //


### Variables locales
>Las variables dentro de las funciones pueden tener un alcance local, eso significa que la variable solo está definida dentro de la funcion

>Y así solo se modifica la variable local, pero no la variable global

> La misma variable puede existir con el mismo nombre pero con diferentes valores dependiendo el alcance, en este caso existiría una en global como: 'nombre' y otra en local como: 'nombre' tambien 

>para referirnos a la variable de alcance global deberíamos especificar dentro de nuestra función:
>```js 
>window.nombre  
>```
>Pero si no es el caso, la funcion siempre tomará la variable local especificada dentro de la misma 

**Toda variable no definida dentro de la funcion, va a estár definida dentro de el alcance global, y vamos a poder definirla dentro de el objeto global**

```js 
console.log("inicializando archivo");
//Imprimiendo algo en la consola

var nombre = "Daniel";
//Una variable global

function imprimirNombreEnMayusculas(nombre) {
// n tiene alcance local
//Para declarar la variable local, simplemente la coloco en parametro 

nombre = nombre.toUpperCase()
//Observaras que puede usar la variable global perfectamente 

console.log(nombre); 
} 
/*
Esta funcion va a tener el efecto colateral de modificar 
la variable nombre
tanto dentro como fuera de la funcion

Esto es algo que queremos evitar en
nuestro codigo \*

imprimirNombreEnMayusculas(nombre);
//De esta manera evito el efecto colateral y tengo un alcance local
```

>nota: en js en general queremos una variable local que no contamine todo el codigo 

Repaso  
¿Que aprendi?  
toda variable que no esta definida en una funcion esta  
definida en el objeto global que en este caso  
en el navegador es window

Aprendi que para crear una variable local asi tenga el mismo nombre que una global tengo que escribir su nombre como parametro en una funcion

Que en javascript en general queremos que una variable local no contamine todo el codigo  
¿Que logre?  
Logre crear una funcion usando tanto variables globales como variables locales

¿Que podre lograr?  
Podre crear un codigo sostenible en el tiempo

Un programador evita efectos colaterales en su codigo

