# ```reduce```
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

>Luego se escrive un ciclo for comenzando en 0 y se le da el parámetro de que mientras que i sea menor a perso