# Iniciando
Dentro de la carpeta **01-hola_mundo** creamos el archivo **"app.js"** en vs code y escribimos una variable con let para el nombre con el valor de "william" y un ```console.log(nombre);``` para tener impreso el nombre en nuestra consola cuando corramos el programa

# Como correr el programa? 
Desde la terminal gracias a node, podemos correr el programa sin tenerlo anexado a otro lado, simplemente con el comando: ```node``` seguido de el nombre de nuestro archivo index que es donde normalmente está la parte del código que inicia el programa (pero en este caso es: ```node app.js```)

# var, let y const (repaso)

### Diferencias 

* Var y let nos permiten definir variables que podemos modificar 

### var
* Tiene un valor por defecto llamado "undefined", puedes no definir el valor de esta variable y solo declararla, y no te va a tirar error, simplemente tien el valor indefinido por defecto, y te permite cambiarlo y modificarlo varias veces con forme avanza el código (aunque no es de las mejores practicas)

### let

Es más especifico para q