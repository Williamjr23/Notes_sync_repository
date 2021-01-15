# Filtrar arrays
### Como filtrar elementos de los arrays?

> Para filtrar siempre se necesitan 2 cosas: 
> * Un array
> * Una condicón 
>> Y esta condición va a ser una ```function```

### ```filter()```
> La función ```filter()``` lleva como parámetro en los parentesís una condicion por ejemplo aquí la condicón sería si la persona es alta o no así que se pondría así:

```js
var personasAltas = personas.filter(esAlta)
```

Y esta condiición ```(esAlta)``` tiene que ser definda como una ```function``` (tiene que ser una ```function```)

### Otra forma de escribirlo
```js
const esAlta = persona => persona.altura > 1.8

var personas = [william, Diana, Parsole, Erick, Elsebasduarte]
var personasAltas = personas.filter(esAlta)

  
///var personasAltas = personas.filter(function (persona) {
///    return persona.altura > 1.8
///})

  

console.log(personasAltas)
```

>

> La forma de abajo es otra manera de hacerlo que también se puede encontrar, pero parece que es un poco más prolijo 