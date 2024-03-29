# Variables: Strings

### Analizando la siguiente linea de código podrémos comprender la aplicación y los valores y nombres que se le da a cada parte de esta misma y aplicarla junto con otras funciones sin que sea la indicada aquí abajo:

> String es una clase en JS que se usa para manipular cadenas de caracteres

Función: **convertir el nombre en mayusculas**:

```js 
var nombreEnMayusculas = nombre.toUpperCase()
```
Desglosando lo anterior:

>Se declara una variable y se le asigna un nombre, de preferencia descriptivo en formato CamelCase:
>```js 
>var nombreEnMayusculas =
>```
>Después se le asigna el valor de nombre que en este caso hace referencia a otra variable donde se define globalmente el nombre sin ningúna modificación:
>```js 
>= nombre. 
>```
>El punto después de definir el valor de nuestra variable se utiliza para invocar una **function** después de esa variable, que en este caso la función para mayusculas sería:
>```js 
>= nombre.toUpperCase()
>```
>y dentro de el paréntesis de esta **functión** se definen los valores de la misma, pero en este caso queremos que se aplique a todo así que no definiremos ningún valor por encima del ya establecido .

Y listo. variable definida, ahora solo faltaría la instrucción para que se muestre en nuestra consola

Lista de funciones y atributos utilizados en esta clase:
>nota: algúnas funciones no necesitan un parámetro para funcionar, los parámetros se definen dentro de los parentesis de la función

| función       | Que hace?                                                                                                                                          |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| toUpperCase() | Convierte a mayusculas                                                                                                                             |
| toLowerCase() | Convierte a minusculas                                                                                                                             |
| charAt()      | Significa caracter en la posición y esta función si requiere un parámetro, el primer caractér de la función siempre empieza desde el número cero 0 |
| substr()      | Acceder a un sub string dentro de un string sus parámetros son el numero de letras simbolos numeros etc a tomar en cuenta dentro de nuestro string | 


| atributo | Que hace?                                                                                                                                                                          |     |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --- |
| length   | a diferencia de las funciones los atributos no se invocan solo nos dan información de algo, en este caso el largo de nuestra palabra o texto representado en un número como output |     |
|          |                                                                                                                                                                                    |     |

Ejemplo de uso en el archivo: **Clase2.js**

### Concatenar strings:
* Interpolación de texto:

>Se emplea con comillas invertidas \`${}\` y lo que esto hace es interpolar variables.
Ejemplo:
>```js 
>   var nombreCompleto = '${nombre} ${apellido.toUpperCase()}' 
>```
>>nota: también podemos observar que con esta forma de concatenar strings nos permite ingresar codigo js dentro de las llaves se puede escribir codigo **Js** con el cual podemos agregar atributos o funciones etc directamente.
>
>En este caso podemos ver que juntamos la variable nombre con la variable apellido de una forma bastante explicativa.

>notas extra: Los strings son cadenas de text. Para indicar que estamos usando una cadena de texto debemos de colocar las comillas simples.
>
>Para concatenar dos strings se utiliza el símbolo (+)  
var nombreCompleto = nombre + ’ ’ + apellido

**Desafío:** Encuentra la última letra de tu nombre