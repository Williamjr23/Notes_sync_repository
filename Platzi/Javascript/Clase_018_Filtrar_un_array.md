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
const esAlta = ({altura}) => altura > 1.8

var personas = [william, Diana, Parsole, Erick, Elsebasduarte]
var personasAltas = personas.filter(esAlta)

  
///var personasAltas = personas.filter(function (persona) {
///    return persona.altura > 1.8
///})

  

console.log(personasAltas)
```

>prolijo: Que se lleva a cabo con detenimiento en los más pequeños detalles

> La forma de abajo es otra manera de hacerlo (se define una ```function``` anonima y luego con las llaves ```{}``` se hace el codigo ahí mismo y funciona de la misma manera) también se puede encontrar, pero parece que es un poco más prolijo tener la condición por separado en lugar de usar una ```function``` anonima 

>El método filter ( ) crea una nueva matriz con todos los elementos que pasan la prueba implementada por la función proporcionada.

>Recuerda que si no hay elementos que pasen la prueba, filter devuelve un array vacío.

>Nota.- De usar una coma sin indicar el valor a tomar al siguiente dato, entonces puede ocurrir algún tipo de error dependiendo el navegador que estés usando, así que deberíamos evitarlo.  El siguiente es un ejemplo de lo que NO debes hacer:
>   ```javascript
>   var valores = [1,2,3];
>  ```

Tarea:
>Escrbir el filtrado de personas bajas