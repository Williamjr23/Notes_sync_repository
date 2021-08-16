Este fue el primer comando con el que inicié mi proyecto
```cmd 
npm init -y
```
> Nos permite crear un proyecto en si (describir que es lo que hace un proyecto )

Instalar dependencias que se van a agregar al proyecto


```
npm i express  express-handlebars morgan firebase-admin
```

> express (fremework de Node que nos va a permitir crear el servidor recibir peticiones y  responder archivos)

>express-handlebars (es un motor de plantillas nos permite extender el html donde no se pueden tener condicionales o bucles, pero con esto ya podremos tenerlo)

>morgan (ver la respuesta de las peticiones al servidor)

>firebase-admin (Driver que nos permite conectarnos a firebase)

## CARPETAS 
### index.js
> Nos sirve para arrancar el prodecto o iniciar el servidor
### App.js
>Configurar el servidor o la applicación 
### Carpeta Views
>Nos servirá para escribir nuestros archivos de html
### Carpeta Routes
>Routes nos servirá para definir las rutas de nuestro servidor
### Public
>Archivos publicos a los que el navegador puede acceder (imagen, archivos, logotipos etc...)

Luego en app se importa el modulo express y luego se utiliza en la siguiente linea, pero aquí no se va a empezar a ejecutar, así que se exporta de app

```js  
const express = require('express');

const app = express();

  

module.exports =app;
```

Después de requerir todos los modulos previamente instalados

```js 
const express = require('express');

const morgan = require('morgan');

const exphbs = require('express-handlebars');
```

El modulo ```morgan``` se le conoce como middleware es por que el modulo va a estar siempre en las peticiones que van a entrar al servidor 