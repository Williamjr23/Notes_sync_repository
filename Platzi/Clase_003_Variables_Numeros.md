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
Explicado por que 
> La forma de trabajar con decimales en JS no es tán precisa de acuerdo a que se estima una cantidad limitada de bytes y para poder hacerlo mas preciso se podría multiplicar x 100 para pasar a un entero y luego dividirlo entre 100 nuevamente después de realizar nuestra operación, pero eso solo funcioina si tiienei un decimal. así que lo mejor será acceder al **modulo** math dentro de js

Ejercicio: clase3.js

