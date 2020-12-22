A que variables pueden acceder y que valores van a tener esas variables

cuando tenemos una variable global?

si una variable no está definida dentro de una funcion, se dice que es de alcance global y eso significa que se puede acceder desde cualquier function

el objeto global en html es la ventana 

esto no siempre es una buena practica, ya que tiene un sideeffect que modifica la variable global y normalmente queremos poder seguir accediendo a ella sin que esté modificada, y esto lo hacemos de la siguiente manera

las variables dentro de las funciones pueden tener un alcance local, eso significa que la variable solo está definida dentro de la funcion

y así solo se modifica la variable local, pero no la variable global

la misma variable puede existir con el mismo nombre pero con diferentes valores dependiendo el alcance, en este caso existiría una en 