# Modelo de caja, valores relativos y absolutos

### Modelo de caja:

> Todos los elementos HTML tienen un modelo de caja, y este modelo de caja está compuesto por 4 elementos: 

1. Contenido: 
> Donde se encuentra el contenido  de nuestra caja todo lo que podamos agregar a esta 
2. Padding: 
> Los paddings siempre nos van a afectar el modelo de caja, eso se tiene que tener siempre presente
3. Border
> Es otra parte de nuestra caja, recubre el padding que a su vez recubre el contenido y como su nombre lo indica, esto es un borde

4. Margin
> Nos funciona para cuando tenemos otros elementos a los lados, las paginas por defecto siempre tienen un margin, y es muy bueno y muy buena practica que nosotros se lo quitemos siempre, para que no se vean afectadas nuestras creaciones en el navegador y esto se hace agregando a nuestro (CSS o style) lo siguiente:

```html
body {
	margin: 0;
}
```

### Las capas del modelo de caja se suman:
> Todas las capas de la caja se van sumando, digamos que el contenido está a 20px (pixeles) y el padding igual a 20px, entonces tendríamos 40px coloreados o indicados en el navegador ya que se suman los del padding mas los de el contenido y así también con el border.
> 
### Como evitar que otras capas modifiquen el tamaño del contenido?
Dentro de nuestra hoja de estilos (CSS) se indíca:
```html
box-sizing: content-box;
```
> "content-box " es el comportamiento CSS por defecto para el tamaño de la caja (box-sizing). Si se define el ancho de un elemento en 100 pixeles, la caja del contenido del elemento tendrá 100 pixeles de ancho, y el ancho de cualquier borde o relleno ser añadirá al ancho final desplegado.

```html
box-sizing: border-box; 
```
> "border-box" le dice al navegador tomar en cuenta para cualquier valor que se especifique de borde o de relleno para el ancho o alto de un elemento. Es decir, si se define un elemento con un ancho de 100 pixeles. Esos 100 pixeles incluíran cualquier borde o relleno que se añadan, y la caja de contenido se encogerá para absorber ese ancho extra. Esto típicamente hace mucho más fácil dimensionar elementos.

Paginas para encontrar colores y agregar a tu página web o programa:
* https://picular.co/Video
* http://paletton.com/#uid=1130u0keOll6mtXaCpdizhfoeei
* https://coolors.co/001514-fbfffe-6b0504-a3320b-e6af2e

>nota: en el navegador casi siempre vamos a trabajar por pixeles, solo en algunos casos puntuales se puede trabajr con otras medidas