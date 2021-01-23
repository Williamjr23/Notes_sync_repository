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
> Lo que vamos a hacer aquí es reducir el array de personas a un total con la function ```.reduce(reducer, 0)```
> Y para reducirlo como parametros dentro de los parentesís necesitamos 2 cosas:
> 1. Una ```function // que en este caso es reducer```
> 2. El valor original o inicial de el acumulador ```0 ```

```
