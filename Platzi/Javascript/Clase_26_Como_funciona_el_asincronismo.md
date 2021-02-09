# Como funciona el asincronismo 



>Js solo puede ejecutar una tarea a la vez y aunque no es multitarea puede delegar los proceso de ejecucuiones a diversas tareas entonces si una funcion llama a otra se van agregando a la pila 

# Callbacks
>Callbacks funciones que ejecutará JS cuando regrese la petición de el servidor

>JavaScript sólo puede hacer una cosa a la vez, sin embargo; es capaz de delegar la ejecución de ciertas funciones a otros procesos. Este modelo de concurrencia se llama EventLoop.

>JavaScript delega en el navegador ciertas tareas y les asocia funciones que deberán ser ejecutadas al ser completadas. Estas funciones se llaman callbacks, y una vez que el navegador ha regresado con la respuesta, el callback asociado pasa a la cola de tareas para ser ejecutado una vez que JavaScript haya terminado todas las instrucciones que están en la pila de ejecución.

>Si se acumulan funciones en la cola de tareas y JavaScript se encuentra ejecutando procesos muy pesados, el EventLoop quedará bloqueado y esas funciones pudieran tardar demasiado en ejecutarse.