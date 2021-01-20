# Transformar Array

### Función: ''``` map() ```''

> Function ```map()``` a diferencia de la function ```filter``` nos va a devolver un nuevo array ```[]``` en el cual va a modificar cada uno de los elementos que le vayamos pasando de el array ```[]``` original

>importante: ```map()``` nos devuelve un nuevo array, pero nos modifica la información y para corregirlo se tiene que retornar un nuevo objeto con la modificación deseada

Ejemplo:

```js
const pasarAlturaACms = persona => {
 return {
 ...persona,
 altura: persona.altura * 100
 }
}
```

>Aquí podemos ver como tenemos que "duplicar" el array al retornarlo con: "```...persona```"" 