# Modelo de caja

> Todos los elementos HTML tienen un modelo de caja, y este modelo de caja está compuesto por 4 elementos: 

1. Contenido: 
> Donde se encuentra el contenido  de nuestra caja todo lo que podamos agregar a esta. (Tambi)
2. Padding: 
> Los paddings siempre nos van a afectar el modelo de caja, eso se tiene que tener siempre presente y esta capa de la caja es la que bordea y separa al contenido del borde.  (Es un relleno al rededor del contenido y también este relleno es transparente por default)
3. Border
> Es otra parte de nuestra caja, recubre el padding que a su vez recubre el contenido y como su nombre lo indica, esto es un borde.

4. Margin
> Nos funciona para cuando tenemos otros elementos a los lados, las paginas por defecto siempre tienen un margin, y es muy bueno y muy buena practica que nosotros se lo quitemos siempre, para que no se vean afectadas nuestras creaciones en el navegador ya que viven en bordes independientes y como veremos mas adelante, estos se suman y va siendo dificil de controlar a menudo que se van agregando objetos, y esto se hace agregando a nuestro (CSS o style) lo siguiente:

```html
body {
	margin: 0;
}
```
>Indicamos que el margen de nuestro body o cuerpo de la página es igual a 0, no es necesario indicar si son pixeles o no, cuando el valor es 0 esto no es necesario.
### Las capas del modelo de caja se suman:
> Todas las capas de la caja se van sumando, digamos que el contenido está a 20px (pixeles) y el padding igual a 20px, entonces tendríamos 40px coloreados o indicados en el navegador ya que se suman los del padding mas los de el contenido y así también con el border.

### Cambiar el tamaño de nuestro margin:
Hay varias formas de cambiar el tamaño de nuestro margin, en primera instancia se puede definir ya sea con: (bottom, top, left, right)
Ejemplo:
```
margin-bottom: 10px;
```

O también, se especifican los margenes de cada lado en uno solo, se tiene que tomar en cuenta que esta opción funciona como las manecillas de el reloj y se especificarán tantas como se deseen ya sea 1,2,3 o las 4 (inicia desde el margen de arriba  y va en sentido de las manecillas del reloj osea: top, right, bottom, left.)
Ejemplo:
```
margin: 10px 20px 30px 40px;
```
>nota: recuerda que el margen por objeto o clase (class) es seteado objeto por objeto y es una propiedad directa de el objeto mismo, así que como lo digimos anteriormente, si tu seteas el margen de tu objeto en 10px, y la página por defecto tiene margen para separar el contenido de los bordes (siempre viene un margen por defecto), este se sumará con el del objeto y suponiendo que este es de 10px también tendrías el borde superior y el borde lateral sumandose a los bordes del objeto adyaciente, esto no quedaría muy parejo y por eso se menciona que es buena practica eliminar estos bordes por defecto y trabajar con los que nosotros querramos dentro de cada objeto o caja.

### Modificar el comportamiento del contenido de nuestra caja:
Dentro de nuestra hoja de estilos (CSS) se indíca ya sea:
```html
box-sizing: content-box;
```
> "content-box " es el comportamiento CSS por defecto para el tamaño de la caja (box-sizing). Si se define el ancho de un elemento en 100 pixeles, la caja del contenido del elemento tendrá 100 pixeles de ancho, y el ancho de cualquier borde o relleno se añadirá al ancho final desplegado.

O también:
```html
box-sizing: border-box; 
```
> "border-box" le dice al navegador tomar en cuenta para cualquier valor que se especifique de borde o de relleno para el ancho o alto de un elemento. Es decir, si se define un elemento con un ancho de 100 pixeles. Esos 100 pixeles incluíran cualquier borde o relleno que se añadan, y la caja de contenido se encogerá para absorber ese ancho extra. Esto típicamente hace mucho más fácil dimensionar elementos.

Paginas para encontrar colores y agregar a tu página web o programa:
* https://picular.co/Video
* http://paletton.com/#uid=1130u0keOll6mtXaCpdizhfoeei
* https://coolors.co/001514-fbfffe-6b0504-a3320b-e6af2e

Esta ultima te indica donde se pueden utilizar los colores:
* https://material.io/resources/color/#!/?view.left=0&view.right=0&primary.color=3F51B5

>nota: en el navegador casi siempre vamos a trabajar por pixeles, solo en algunos casos puntuales se puede trabajar con otras medidas.

Notas extra:

>Una buena practica es normalizar nuestro proyecto (eliminar los márgenes que vienen por defecto, entre otras cosas)

>Es bueno aprender a hacerlo pero agregando este archivo nos facilita todo ese proceso.
https://necolas.github.io/normalize.css/
Al Agregar el link en nuestro index o archivo.html debe ir primero que el link de la hoja de estilos principal para que no se vea afectado lo que estemos haciendo o definiendo.