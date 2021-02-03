# Modificando un prototipo
>### Prototipos diferentes a el sistema de herencia en otros lenguajes de programación:
>>JavaScript provoca cierta confusión en desarrolladores con experiencia en lenguajes basados en clases (como Java o C++), por ser dinámico y no proporcionar una implementación de clases en sí mismo (la palabra clave `class` se introdujo en ES2015, pero sólo para endulzar la sintaxis, ya que JavaScript sigue estando basado en prototipos
>
>Mas info [Herencia y la cadena de prototipos](https://developer.mozilla.org/es/docs/Web/JavaScript/Herencia_y_la_cadena_de_protipos)

# Prototipo como objeto
>El ```prototype``` es un objeto más de JS entonces si se modifica a una cierta altura, a partir de ahí se va a quedar modificado
>> En este caso se refiere a que no se puede definir un ```prototype``` después de invocarlo ya que Js detiene el codigo al tener un error y si el prototipo se define después de requerirlo se va a detener el codigo antes de llegar a este mismo
>
>Por eso es una buena practica intentar que todos nuestros ```prototype``` estén mayormente juntos
>>nota: Es muy importante donde colocamos las funciones que va a tener el prototipo y siempre colocarlas todas juntas.

# Definiendo prototipos como arrow functions
> La forma de utilizar ```this.``` dentro de las arrow functons es diferente a como sería normalmente y se hablará de su función y la forma de eje