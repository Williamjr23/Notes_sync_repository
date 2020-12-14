# Posicionamiento en CSS

El posicionamiento en CSS es una de las cosas más importantes, pues establece cómo van a estar ubicados nuestros elementos en la pantalla.

En CSS los elementos se posicionan utilizando las propiedades top (superior), bottom (inferior), left (izquierda) y right (derecha), pero sólo funcionarán si la propiedad position está establecida. Esto quiere decir que si quiero que mi elemento div esté completamente a la derecha, debo escribir en mi CSS lo siguiente:

```CSS
div { position: absolute: right: 0px; }
```
La propiedad **position** tiene 7 valores diferentes: relative, absolute, fixed, sticky, static, initial e inherit. Veremos de qué se tratan:

| propiedad y valor  | Descripción                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Position: relative | El elemento se coloca en relación a su posición normal.                                                                                                                                      |
| Position: absolute | Los elementos con esta posición se ubican en relación al elemento relativo más cercando. Aquí podemos hacer uso de las propiedades top, bottom, left y right.                                |
| Position: fixed    | El elemento se ubica en relación con la ventana del navegador y también se ve afectado por las proiedades top, bottom, left y right.                                                         |
| Position: sticky   | El elemento se posiciona en función de la posición de desplazamiento del usuario. Si lo ubicas a la izquieda, siempre va a estar ahí sin importar cuántas veces se haga scroll en la página. |
| Position: static   | Los elementos HTML son estáticos por defecto, siguen el flujo normal de la página y no se ven afectados por las propiedades top, bottom, left y right.                                                                                                                                                                                             |
