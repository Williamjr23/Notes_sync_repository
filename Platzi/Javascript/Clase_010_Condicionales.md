# Estructuras de control
> nos van a permitir decidir si un codigo se ejecuta o no se ejecuta, multiples veces o hasta que se cumpla cierta condición

### Primera estructura de control que vamos a ver:
1. Condicionales
> en la cual vamos a definir justamente si un codigo se ejecuta o no 

> Lo que vamos a hacer en esta practica es: definir una función que nos va a decir que profeciones va a tener una persona, aquí estamos trabajando con valores booleanos de ```true``` or ```false``` así que de esta manera es como podremos decir internamente en el codigo si es verdadera la sentencia de codigo o no lo es

```js
console.log(`${persona.nombre} es:`) 
```
>Esto se llama temple string y es como lo vimos anteriormente una forma de interpolar variables, se utiliza la comilla invertida y la expresión de la siguiente forma:
>```js
>(`${persona.nombre}`)
>```
> y todo lo que abarque las comillas estará dentro, también recordar que es con comillas invertidas y al decir que se pueden interpolar variables, esto se refiere a que se pueden concatenar direcciones a objetos como en el caso anterior o sacar outputs directamente desde el string


para decir que la instrucción que demos a la ```function``` se haga dependiendo de si se cumple cierta condición en este caso utilizamos el primer condicional que es el ```if() { }```, dentro de los parentesis se indica la condición y todo lo que esté dentro de las llaves ```{}``` es lo que se va a ejecutar si y solo si se cumple la condicional y se vería de la siguiente manera:


```js 
function imprimirProfesiones(persona) {
console.log(`${persona.nombre} es:`)
// if (persona.ingeniero === true)
if (persona.ingeniero) {
console.log('Ingeniero')
 }
}
```
>nota: Aquí vemos que no hace falta preguntar si ``` // if (persona.ingeniero === true) ``` por que ya con el if ya estamos diciendo que tiene que ser true así que se utiliza la otra forma.

### cuando el valor es falso y se quiere responder:

Ahora para el codigo que no se va a ejecutar se va a utilizar despues de el if que sería la traducción sí, el condicional else que se podría traducir como entonces 

Se utiliza el ```else```

escribir la function llamada imprimir si es mayor de edad y va a recibir una persona, y lo que quiere que imprima es si sacha es mayor de edad, o es menor de edad, tomando en cuenta como edad 18 años 

```js
function imprimirSiEsMayorDeEdad(persona) {
// Sacha es mayor de edad
// Sacha es menor de edad
}
```

recordar utilizar los operadores para comparar numeros > < >= <=

Cosas aprendidas en la clase:
* escribir condicionales