# ```function``` ```prototype``` a arrow function
Quien es tihs?

aqui nos dice que this es window

y window es el objeto global dentro de el navegador 

y como dentro de los parametros de el objeto global "window" no está lo que estamos referenciando dentro de nuestro codigo nos aparecerá normalmente "undifined", y esto es uno de los errores mas comunes en JS tanto en el backend como en el frontend, la función ```this.``` no siempre va a estar referenciando el objeto que esperas que esté referenciando, este es uno de los casos representado al intentar hacer nuestra linea de codigo anterior en una arrow function

// codigo 1 y 2j

como podemos ver aquí en las arrow functions this no es lo que esperabamos y lo que pasa aquí es que asigna esa function pero a
