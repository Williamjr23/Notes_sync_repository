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

Y esto te ahorra el trabajo de tener que configurarlo tu mismo para cada dispositivo