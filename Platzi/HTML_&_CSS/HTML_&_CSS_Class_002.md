# Anatomía de un documento HTML

> *nota: al editar codigo HTML desde VScode, se recomienda indicar que se está trabajando con HTML para que así el editor reonozca nuestro codigo al editarlo y nos pueda sugerir, reconocer y marcar las cosas que nos facilitan la lectura y escritura del mismo (esto se indica guardando el archivo al iniciar con la extención "HTML")*

Iniciamos dentro de VScode y de las primeras cosas que entramos es:
 ```html
 html:5 
 ``` 
 Esto nos va a abrir el siguiente preset de codigo HTML:
 ```html
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html> 
 ``` 
 
En el caso anteriór la etiqueta "meta" con el atributo "viewport" sirve para definir la escala visual del sitio.

En pocas palabras si defines también el atributo "content" después del atributo "viewport" en la misma etiqueta meta con el valor: **"width=device-width, initial-scale=1"** le estamos diciendo a nuestro sitio web que ancho máximo de nuestra página web será el ancho del dispositivo desde donde se esté aperturando el sitio web (móvil, tablet, pc).

Y esto te ahorra el trabajo de tener que configurarlo tu mismo para cada dispositivo, practicamente le estás dando los parámetros de que tu sitio de escritorio así como lo visualizas tu se transporte hacia cualquier dispositivo de una manera orgánica, pero si por otro modo quisieras saber un poco mas a cerca de como personalizarlo en los diferéntes dispositivos está este [artículo](https://blog.hubspot.com/marketing/mobile-viewport-setup) que te podría interesar para saber mas a fondo como funciona
	
Luego con la etiqueta <!DOCTYPE html> se está indicando que el documento está utilizando html

A partir de aquí ya no nos tenemos que preocupar tanto por la anatomía o estructura principal de nuestra página, ya que esto nos permite simplemente empezar a escribir directamente desde el body y agregar lo que necesitemos a partir de aquí nuestra página ya puede mostrarse

# Anatomía de un documento HTML

> *nota: al editar codigo HTML desde VScode, se recomienda indicar que se está trabajando con HTML para que así el editor reonozca nuestro codigo al editarlo y nos pueda sugerir, reconocer y marcar las cosas que nos facilitan la lectura y escritura del mismo (esto se indica guardando el archivo al iniciar con la extención "HTML")*

Iniciamos dentro de VScode y de las primeras cosas que entramos es:
 ```html
 html:5 
 ``` 
 Esto nos va a abrir el siguiente preset de codigo HTML:
 ```html
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html> 
 ``` 
 
 En este caso empezamos viendo como funciona cada una de las etiquetas y el por que nos las está poniendo automaticamente y veremos por que esto nos ahorra tiempo.
 
 La primera etiqueta es:
 
 ```html
 <!DOCTYPE html>
 ```

El Doctype o “Declaración del tipo de documento” es una instrucción especial que va al inicio de nuestro documento HTML y que permite al navegador entender qué versión de HTML estamos utilizando. Esta información determinará la manera en la que el navegador procesará el documento, un DOCTYPE distinto podría implicar hasta una visualización diferente del sitio web dentro del mismo navegador.

La siguente etiqueta es:
```html
<html lang="en"> 
```

Se usa casi siempre un atributo de idioma en la etiqueta html para declarar el idioma predeterminado del texto de la página. Cuando la página tenga contenido en otro idioma, agregue un atributo de idioma a un elemento que rodee a ese contenido.

Y si la página está en varios idiomas diferentes de preferencia debe ser indicado y para esas diferentes opciones puedes consutlar mas detalles [aquí](https://www.w3.org/International/questions/qa-html-language-declarations.es)

Luego tenemos: 
```html
<meta charset="UTF-8"> 
```

El elemento **meta** con atributo **charset** en un documento HTML está destinado a indicar la codificación de caracteres utilizada 

Por ejemplo, si se utiliza la codificación UTF-8 (estándar en HTML5 reconocido por la RFC 3629 de la Internet Engineering Task Force (IETF) y una de las tres posibilidades de codificación reconocidas por Unicode)

Luego:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

