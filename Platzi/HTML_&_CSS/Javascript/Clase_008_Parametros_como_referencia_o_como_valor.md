# Parametros como referencia o valor

>nota de clase: Javascript se comporta de manera distinta cuando le pasamos un objeto como parámetro.

Cuando los objetos se pasan como una referencia, estos se modifican fuera de la función. Para solucionar esto se puede crear un objeto diferente. Esto lo podemos hacer colocando tres puntos antes del nombre. Ej …persona.

### Modificar una variable global o un objeto desde el cuerpo de una function:

>nota: este modo de trabajar con las funciones tiene el efecto de lado (sidefect) de que se modifica la variable global o los atributos dentro de un objeto, esto puede ser util si es que se necesita para algo, pero si no se necesita para algo, esto puede ser una mala practica, ya que influye de manera directa con nuestro objeto 

> JS se comporta diferente con los objetos, los objetos que pasamos por parametros se pasan por referencia, 

> osea que si los modificamos dentro de el cuerpo de una funcion, su valor se va a ver modificado de fuera de esa función también 

Ejemplo:
```js
// modifica el valor de el atributo interno del objeto 

function cumpleanos(persona) {

    persona.edad += 1

}
```

En este caso esta ```function``` está modificando el atributo **edad** dentro de el objeto **william** así que cada vez que invoquemos la ```function``` cumpleanos se sumará 1 a la edad de el objeto que se le indique, ya sea en este caso el objeto william o el objeto russel, y se tiene que especificar en este caso que objeto es al que le tiene que hacer la modificación y en este caso podría ser:

```js 
cumpleanos(william)

// o también podría ser:

cumpleanos(russel)
```

### Evitar que se modifique la variable global o los atributos de un objeto al usar una function

> se puede devolver un nuevo objeto con ```return``` dentro de nuestra function, que en este caso lo que va a hacer es devolvernos (return) un nuevo objeto que tiene todas las características de nuestro objeto principal, solo que con la diferencia que dentro de la functión se le está cambiando, agregando, suplantando algúna  o varias carácterísticas especificas y ese sería nuestro nuevo objeto. es decir:

Esto lo que hace es devolvernos un nuevo objeto hecho completamente igual a base de la persona pero dentro de los atributos de return especificamos que se modifique unicamente la cracterística edad dentro de el objeto retornado en la variable, asi que tenemos un objeto igual al global, pero sin afectar las variables del objeto global y con el output modificado
```js 
function cumpleanos(persona) {
 return{
 ...persona,
 edad: persona.edad + 1
 }
} 
```

> A los tres puntos “…” se llama _operador de propagación_ (**Spread operator**), es una nueva implementación en **ES6**. Básicamente lo que hace es crear un duplicado de nuestro objeto para luego modificarlo según lo que necesitemos.

> Si tienes pensado usar tecnologías como Flux o Redux, pon mucha atención a este video. Nunca debes modificar el estado del objeto sino crear otro.
