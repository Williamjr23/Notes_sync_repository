A que variables pueden acceder y que valores van a tener esas variables

cuando tenemos una variable global?

si una variable no está definida dentro de una funcion, se dice que es de alcance global y eso significa que se puede acceder desde cualquier function

el objeto global en html es la ventana 

esto no siempre es una buena practica, ya que tiene un sideeffect que modifica la variable global y normalmente queremos poder seguir accediendo a ella sin que esté modificada, y esto lo hacemos de la siguiente manera

las variables dentro de las funciones pueden tener un alcance local, eso significa que la variable solo está definida dentro de la funcion

y así solo se modifica la variable local, pero no la variable global

la misma variable puede existir con el mismo nombre pero con diferentes valores dependiendo el alcance, en este caso existiría una en global como: 'nombre' y otra en local como: 'nombre' tambien 

para referirnos a la variable de alcance global deberíamos especificar dentro de nuestra función:

```js 
window.nombre 
```

pero si no es el caso, la funcion siempre tomará la variable local especificada dentro de la misma 

toda variable no definida dentro de la funcion, va a estár definida dentro de el alcance global, y vamos a poder definirla dentro de el objeto global

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
Esta funcion va a tener el efecto colateral de modificar la variable nombre tanto dentro como fuera de la funcion Esto es algo que queremos evitar en nuestro codigo \*/ imprimirNombreEnMayusculas(nombre); //De esta manera evito el efecto colateral y tengo un alcance local
```