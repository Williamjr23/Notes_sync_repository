# OOCSS, BEM, SMACSS, ITCSS y Atomic Design

1. **OOCSS** (CSS Orientado a Objetos)
> Separa el diseño de el contenido y así se puede reutilizar muchisimo mejor el codigo
 
Ejemplo:
```html 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    body {
        margin: 0;
    }
    .globalwidth {
        width: 100%;
    }
    .header {
        background-color: goldenrod;
        height: 50px;
        margin-top:0;
    }
    .footer {
        background-color: pink;
        height: 25px;
    }
</style>
<body>
    <header class="header globalwidth"><H1>Header</H1></header>
    <footer class="footer globalwidth">Footer</footer>
</body> 
</html>
```
> Aquí podemos ver como separamos el width que e el mismo para el ```footer``` que para el ```header```  en una clase por separado para poderlo utilizar como clase secundaria en ambas etiquetas y así optimizar el codigo y no replicarlo, aquí se puede ver un ejemplo de como esta clase es reutilizable.

2. **BEM** (Block Element Modifier)
> separa los bloques, los elementos y modificadores (su nombre es una abrebiatura de sus compuestos; Bloque, Elemento, Modificador)

* Bloque
>Entidad independiente que es significativa por sí misma.
>
Ejemplos:
```header``` ``` container ```  ```menu```  ``` checkbox```  ```input```

* Elemento
> Parte de un bloque que no tiene un significado independiente y está semánticamente ligada a su bloque.
Ejemplos
```menu item``` ```list item``` ```checkbox caption``` ```header title```

* Modificador
> Una bandera en un bloque o elemento. Úselos para cambiar la apariencia o el comportamiento.
Ejemplos
```disabled```  ```highlighted``` ```checked``` ```fixed``` ```size big``` ```color yellow```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BEM</title>
</head>
<style>
</style>
<body>
    <header class="header">
        <button class="header__button--red">Red</button>
        <button class="header__button--yellow">Yellow</button>
    </header>
</body>
</html>
```

>En este caso: "header es el bloque, button es el elemento y red" es el modficador.

3. ** SMACSS** (Arquitectura de CSS escalabl y modular) 
> Se divide en 5 Pasos:
	>1. Base
	>>Componentes base, elementos a utilizar en toda la app, como los botones
	>2. Layout
	>>Elementos que se utilizan en la página una sola vez como el hader o e footer
	>3. Module
	>>Componentes que se utilizan en la applicación mas de una vez
	>4. State
	>>Acciones de nustros componentes
	>5. Theme
	>> No todas las applicaciones tienen temas, pero la idea es que facilite la forma de cambiar de tema o de trabajar con estos

4. ** ITCSS**  (Triangulo invertido de CSS)
> Poder dividir todos los archivos de nuestro CSS en ciertas partes para que no se combinen entre si y el orden es en tipo piramide invertida así que va en descenente en el siguiente orden:
> * Ajustes
> * Herramienas
> * Generico
> * Elementos
> * objetos
> * Componentes
> * Utilidades

> Y se acomodan con forme magnitud, especificidad y claridad

5. ** Atomic Design** (Diseño atómico)
> Lo separó en Átomos, Moléculas, Organismos, para hacer templates y páginas.

Dejo aquí las siguientes páginas para leer a cerca de estas tecnoloías respectivamene:
* [oocss](https://www.smashingmagazine.com/2011/12/an-introduction-to-object-oriented-css-oocss/)
* [BEM](http://getbem.com/introduction/)
* [SMACSS](http://smacss.com)
* [ITCSS](https://www.xfive.co/blog/itcss-scalable-maintainable-css-architecture/)
* [atomic design](https://bradfrost.com/blog/post/atomic-web-design/)