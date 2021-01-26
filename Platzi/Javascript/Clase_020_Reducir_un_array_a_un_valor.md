# Reducir un valor a un array
> Reducir un array a un valor unico

> Se puede hacer de la siguiente manera como y lo vimos anteriorment con los ciclos ```for```, pero esta no es la mejor manera de hacerlo, igual esta forma de hacerse debajo de el codigo :

```js
var acum = 0

for (var i = 0; i < personas.length; i++) {
 acum = acum + personas[i].cantidadDeLibros
}

console.log(`En total todos tienen ${acum} libros`)

```

> Se crea un acumulador "```var acum = 0```" que empieza en 0 

```js 
for (var i = 0; i < personas.length; i++) {}
```
>Luego se escribe un ciclo ``` for() ``` comenzando nuestro contador en 0 ``` var i = 0;``` y se le da el parámetro de que mientras que i sea menor a personas. length se va a ir repitiendo el ciclo ```i < personas.length; i++```

>```acum = acum + personas[i].cantidadDeLibros```
>Aquí estamos diciendo que a nuestro acumulador se le van a sumar "Personas sub indice i y la cantidad de libros"

# ```reduce```


> Otra forma de hacer lo anterior
 ### Como funciona?
 
 
```js
 var totalDeLibros = personas.reduce(reducer, 0 )

console.log(`En total todos tienen ${totalDeLibros}`)
``` 

> En este caso tenemos la forma de usar y definir los parametros de ```reduce```

> Lo que vamos a hacer aquí es reducir el array de personas a un total con la function ```.reduce(reducer, 0)```
> Y para reducirlo como parametros dentro de los parentesís necesitamos 2 cosas:
> 1. Una ```function // que en este caso es reducer```
> 2. El valor original o inicial de el acumulador ```0 ```

### Definiendo la funcion reducer 
> Esta function le va a dar instrucciones para que reduce sepa que retornar a la hora de que se cumpla la condición establecida en esta misma functión:
```js
const reducer = (acum, persona) => {
return acum + persona.cantidadDeLibros}
```

> Como vemos es una arrow function que nos recive 2 parámetros y en primer lugar recive el acumulador ```acum``` y en segundo lugar va a ir recibiendo cada uno de los elementos y en este caso cada una de las personas ```persona```

> Posteriormente se modifica el valor que quieres que tenga el nuevo acumulador ```return acum + persona.cantidadDELibros```

También como ya lo hemos visto anteriormente se puede desestructurar el objeto dentro de los paréntesis con llaves y así solo acceder a persona y implicitamente ya sabe que tiene que tomar ```cantidadDeLibros``` de el objeto que le digamos a continuación, también como vimos en la clase **arrow functions** ya que solo nos returna un valor se puede obviar la palabra ```return```y quitar las llaves, y nuestra linea quedaría así:

```js
const reducer = (acum, {cantidadDeLibros}) =>
acum + persona
```

Y esto hace exactamente lo mismo que el ejemplo anterior.

