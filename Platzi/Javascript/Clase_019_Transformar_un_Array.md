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

>Aquí podemos ver como tenemos que "duplicar" el array al retornarlo con: "```...persona,```" y posteriormente definir la ```altura:``` de ese nuevo arreglo clonado de el original y aquí si podríamos modificar entonces los datos sin que se vea afectado nuestro objeto global y por ende nuestro arreglo y ahora sí se define ``` altura: persona.altura *100``` y al consultar la ```function``` ```pasarAlturaACms``` entonces tendríamos nuestro arreglo duplicado y modificado con los valores que tengamos en el.  

```js
var personasCms = personas.map(pasarAlturaACms)
```

>Por ultimo solamente se define una varable en este caso ```personasCms``` donde nuestro arreglo de ```personas``` utilce la función ```map()``` para devolver un nuevo array con las modificaciones especificadas anteriormente en ```pasarAlturaACms```