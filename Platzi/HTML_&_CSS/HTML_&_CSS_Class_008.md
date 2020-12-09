# Tipos de selectores, pseudo-clases y pseudo-elementos

### Tipos de selectores:

* Universal
> Se aplica con un asterisco "*"  (con esta opción se aplican las propiedades a todos los elementos html) 

> Ejemplo:
> ```html
> * {
>	margin 0; 
>	 } 
> ```

* Tipo
> Se aplican a etiquetas para cambiar los atributos en todas las veces en las que esté presente esa etiqueta en nuestro código

> Nota: (no son tan buenos y no se recomienda utilizarlos cuando estamos trabajando en aplicaciones muy grandes o con muchas hojas de estilo o con muchos estílos, por que si lo aplicas por ejemplo aun parrafo se van a colorear todos los parrafos y no siempre se quiere que eso pase)

> Ejemplo:
> ```html
> h1 {
>      color: red;
>      } 
> ```

* Clase
> Se colocan atributos a los eleméntos, aquí se coloca un identificador a nuestros elementos para poderlos trabajar dentro de CSS y especificar por ejemplo que el titulo principal tiene un color, un formato y el pie de página otro etc...

>Ejemplo:
>```html
>. saludo { 
>      font-size: 2cm;
>          }
>```

* ID
>Se conocerá mas adelante pero se indica por que pertenece a los tipos de selectores

>Nota: (Tampoco es muy bueno ni tan recomendable trabajar con IDs, mas adelante se hablará sobre la especificidad y se verá por que no es tan bueno trabajar con IDs>

> Ejemplo:
> ```html
> # id {
>     border-radius: 20px;
> }
> ```

### Pseudo-clases:
Si se quiere aplicar un estilo en especial (el primer parrafo, el segundo parrafo, el ultimo, numeros pares o impares, etc...) para eso están las "Pseudo-clases" y estas nos van a dar estílo específicos y aquí mencionaremos algúnos cuantos:

* First Child (Primer_hijo):
```html
p:first-child 
	{
	color: white;
	}
```
> La pseudo-clase :first-child de CSS representa el primer elemento entre un grupo de elementos hermanos. ya sea que si se aplicará al primer elemento de la lista y a cada primer subelemento de la misma.

* Last Child (Ultimo_hijo):
```html
p:last-child 
	{
	Color:purple;
	}
```
> Esta nos permite que se modifique el estilo a el ultimo hijo de cada elemento seleccionado y a sus sub eleméntos.

* Para Pares:
```html
p:nth-child(2n)
	{
	color:red;
	}
```
> Aquí se le indíca que todos los numeros de 2 en 2 osea los pares de el elemento se les aplique un estílo especifico.

> nota: "n" nos indica un numero cualquiera y "th" hace alusión a los números ordinarios en inglés 

* Para impares:
```html
p:nth-child(2n+1)
	{
	color:red;
	}
```
Hay mas formas de hacerlo sin utilizar expresamente las matemáticas, pero esta es la base de como funciona el indicar que se aplique un estilo sin necesidad de seleccionar elemento por elemento

### Pseudo-elementos:
```html
::
```
Su sintaxis son dos puntos "::" antes, despues de seleccionar lo que queramos puntualmente cambiar, como un solo caracter a la vez modificar el color o el tamaño del mismo,

Consultar: Ejercicio_005.html