# Variables Números	
### Incremeto: (conocido como suma para que te des una idéa, pero le llamaremos incremento)

para incrementar el valor de una variable hay varias formas:

1. Simple
```js 
edad = edad + 1 
```

2. Recortada
```js 
edad += 1 
```

Se hace de la misma manera con disminuir (o tambíen conocido como sustracción)

### Variables numéricas:
> Se tiene que tomar en cuenta que se puede asigan un valor numérico a una variable con un nombre en texto así como lo hemos hecho con los strings, pero así mismo como hemos mencionado a cerca de JS como un lenguaje debilmente tipado, tenemos que tener algo de cuidado con que estas variables si van a ser numeros no se conviertan en strings

Ejemplo:

```js 
var edad = 18

var peso = 61
```

>Nota: tratar de que se queden las variables de numeros solo en numeros y no agregar kg o años dentro de la variable, en todo caso al invocarlas se puede agregar de diferentes maneras para mantener un codigo limpio y con esto nos referimos a no transformar una variable numerica en un string ya que a la vez se hace mas complicado trabajarla:
>```js 
>  var 
>```
### Decimales
Explicación
> La forma de trabajar con decimales en JS no es tán precisa de acuerdo a que se estima una cantidad limitada de bytes y para poder hacerlo mas preciso se podría multiplicar x 100 para pasar a un entero y luego dividirlo entre 100 nuevamente después de realizar nuestra operación, pero eso solo funcioina si tienes un decimal.

Ejemplo:
```js
var total = precioDeVino *100 *3 / 100
```

Formá sencilla de hacerlo:
>   Así que lo mejor será acceder al **modulo global** ```math``` dentro de js y seguido de la instrucción: ```.round``` lo que le indíca que se redondea la cantidad final.
 
Ejemplo:
```js
var total = Math.round(precioDeVino *100 *3) / 100
```

Para que el output de tu decimal sea exactamente de el largo que tu quieres sería especificandoselo como de la siguiente manera:
```js
var totalStr = total.toFixed(2)
```
 y lo anterior es un string, para volver a decimal se utiliza:
 ```js 
 var total2 = parseFloat(totalStr) 
 ```
> nota: esto convierte de string a decimal

### Divición:
Ejemplo:
```js
var pizza = 8
var personas = 2
var cantidadDePorcionesPorPersona = pizza / personas
```



Ejercicio: clase3.js

