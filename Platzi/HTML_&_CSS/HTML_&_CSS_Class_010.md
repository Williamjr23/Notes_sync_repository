# Valores relativos y absolutos
### Unidades de medida absolutas:
* cm (centimeters)
* in (inches)
* px (pixels)
* mm (milimeters)
* pt ()
* pc()

### Unidades de medida relativas:
* vmax
* em
* ch
* ex
* rem
* vmin
* vw
* vh

En las unidades relativas, el tamaño de nuestro objeto en este caso depende de el dispositivo desde el que se está mostrando
Ejemplo:
```html
<style>
	header {
		bacground-color: #21C98B;
		width: 100%;
		height: 80px;
	}
</style>
```
> En este caso solamente el "width:" está establecido con una unidad relativa, en este caso siendo el porcentaje "%" y así indicamos que se muestre desde donde se muestre el ancho siempre va a llenar el 100% de la página para el header, y que de alto para el header solo usará, se muestre donde se muestre el valor absoluto de 80px (pixeles).

>Nota: En el caso del codigo anterior el header no ocupa todo el espacio de la página desde el inicio, así que recordando notas anteriores como buena practica se quita el margen por defecto del cuerpo de nuestra página (body) dentro de la etiqueta style de la siguiente manera:
```html
	body
```