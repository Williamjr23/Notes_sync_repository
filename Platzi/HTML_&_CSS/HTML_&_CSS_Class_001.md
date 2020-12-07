# Anatomía de un elemento HTML, atributos, anidamiento y elementos vacíos (conceptos iniciales de html)


### Anatomía de un elemento HTML:

Este es un ejemplo de elemento HTML:
 ```html
 <h1> hola </h1> 
 ```

Y se compone de:

Etiqueta de apertura:
 ```html
 <h1> 
 ```

Contenido:
 ```html
 hola 
 ```

Etiqueta de cierre: 
 ```html
 </h1> 
 ```

### Atributos:
En este caso tenemos el atributo "class" que nos da un identificador a cada elemento para luego en CSS podamos definir que estilos va a tener esa clase "class" y la parte de "Saludo" en este caso es el valor que se le va a dar a esa clase:
 ```html
 <h1 class= "Saludo" > 
 ```
>*Nota: Los atributos **siempre** van en la etiqueta de apertura*

### Anidamiento

Puede haber etiquetas dentro de otras, elementos dentro de otros 

Un ejemplo de etiquetas anidades puede ser:

 ```html
<ol>
  <li>Elemento 1</li>
  <li>Elemento 2</li>
  ...
  <li>Elemento N</li>
</ol>
 ```

Tanto listas ordenadas como listas desordenadas son un buen ejemplo de esto, y como podemos se indica que tipo de lista va a hacer y se especifica dentro de se anida dentro de la etiqueta otra etiqueta para indicar elementos dentro de la lista y al final se cierra de nuevo la etiqueta principal

### Elementos vacíos

En este caso tenemos como indicarle al navegado en todo caso de que pase algo por ejemplo cun una imágen y no se pueda renderizar o visualizar, se llama elementos vacíos por que al no haber cargado el elemento deseado se cargará lo que se ponga aquí

Ejemplo:
 ```html
<img src="puppy.png" alt="mi mascota" > 
 ```
 
 ad
