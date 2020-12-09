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
>