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
>Se conocer

>Nota: (Tampoco es muy bueno ni tan recomendable trabajar con IDs, mas adelante se hablará sobre la especificidad y se verá por que no es tan bueno trabajar con IDs>

> Ejemplo:
> ```html
> # id {
>     border-radius: 20px;
> }
> ```
