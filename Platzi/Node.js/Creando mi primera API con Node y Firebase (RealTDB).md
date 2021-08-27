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
> Nos sirve para arrancar el proyecto o iniciar el servidor
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

```js 
// settings

app.set('port', process.env.PORT || 3000);
```

Con la anterior configuración se definió el puerto ahí dice que si en el sistem 
existe algún puerto definido para la app lo toma, y en el caso que no exista usa el número 3000

## Modulo path 
```js 
const path = requiere('path');
```
Importando el modulo path nos permite trabajar con los directorios, viene por defecto dentro de node 

```js 
app.set('views', path.join(__dirname, 'views'));
```

Nos permite combinar 2 directorios o 2 rutas de carpetas ```__dirname``` nos da la ruta entera de en donde está la carpeta desde el sistema operativo ( en este caso la ruta llega a src) y luego combina con el nombre "views " (con esa linea de codigo le decimos a node que la carpeta view está disponible  y donde encontrarla )

```js 
app.engine('.hbs', exphbs({

 defaultLayout: 'main',

 extname: '.hbs'

}));
app.set('view engine', '.hbs');
```

me permite configurar el motor, default layout define codigo en común que se va a poder reutilizar  y el extname: '.hbs' define las extensiones que vamos a utilizar como .hbs de lo contrario tendríamos que usar la extención "handlebars", simplemente es para hacerlo más corto y legible 

con la ulitma linea de aquí que sería:
```JS 
app.set('view engine', '.hbs');
```

Ya dejamos de definir el motor y con esta linea se empieza a utilizar el motor 
```js 
//middlewares

app.use(morgan('dev'));

app.use(express.urlencoded({extended: false}));
```
Definimos que queremos que utilice el modelo morgan y que lo ejecute, y el dev es un valor que nos pide, en este caso es dev por que está en desarrollo 

luego ejecutamos express es para que podamos recibir formularios que nos lleguen de peticiones html y en este caso con el false, solo se reciben datos en Json

```js 
npm i nodemon -D
```
Se instala para que se reinicie el servidor automáticamente cada que guardamos un cambio 

 ```js
const { Router } = require('express');
const router = Router();


module.exports = router;
 ```
 
 Aquí empezamos a requerir una parte de express que se llama enrutador, y un enrutador lo que nos permite es crear rutas para mi servidor 
 
 Y lo que estamos diciendo en las lineas de código sería:
 
 voy a requerir desde el modulo express un enrutador (un metodo llamado router)
 y abajo lo ejecutamos y al ejecutarlo nos devuelve un objeto y este objeto es el que vamos a exportar, y este objeto va a ser el que vamos a llenar de rutas 
 
 ```js 
const router = Router();

router.get('/', (req, res) => {

})
 ``` 
 Aquí creamos una función que acepta 2 parámetros (request y response) son 2 objetos que me dan información sobre la petición y la respuesta 
 
 ```js 
 // routes / index.js 
 const admin = requiere('firebase-admin');
 ```
 Aquí requerimos el modulo previamente importado al proyecto en el "package.json" llamado ```firebase-admin``` y este modulo se tiene que configurar,  no es tan solo llamarlo y dejarlo ahí, entonces lo guardamos en una constante llamada ```admin``` 
 
 ```js 
 const admin = requiere('firebase-admin');

admin.initializeApp({
credential: admin.credential.applicationDefault(),
databaseURL:''
})
 ```
 Aquí especificamos 2 cosas, con: ```admin.initializeApp({})``` es como decir "voy a inicializar una aplicación" y dentro de esto, se van a especificar las credenciales, que en este caso ```credentaia