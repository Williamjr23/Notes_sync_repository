# Funciones que retornan valores

En la clase de hoy vimos "Funciones que retornan valores" y con esto se refiere explicitamente a desglozar el funcionamiento de una función en otra que nos returne ```return``` un valor en este caso es true o false, el anterior código que nos resolvía todo en una sola functión, ahora para volverlo mas explicito mejor manejable mas visual y escalable, desglosamos el valor de mayor de edad en una ```function``` de la siguiente manera:

```js
function esMayorDeEdad(persona) {
 return persona.edad >= MAYORIA_DE_EDAD
}
```

### constantes
Va a haber momentos en los que un tipo de dato o variable necesite ser mas que variable, una constante, lo que significa que no se debe modificar, siempre va a permanecer con el mismo valor, y a pesar de que podemos darle un valor como ```var```variable, lo mejor será darle el valor de ```const```constante para especificar que ese tipo de dato siempre va a permanecer así y no debe cambiar.

Ejemplo:
```js
const MAYORIA_DE_EDAD = 18 
```

>nota: para las ```const``` en lugar de utilizar **camelCase** como lo hacemos en ```var```, esta vez utilizaremos el escribir la constante con TODAS_LAS_LETRAS_MAYUSCULAS, como una buena practica para distinguir las constantes de las variables de manera sencilla.

Para terminar, se desglozó la función para que fuera mas sencillo trabajar con ella y se pudieran reutilizar los valores o constantes en dado caso de que sea necesario, es importante siempre intentar hacer que nuestro codigo esté lo mas limpio posible 