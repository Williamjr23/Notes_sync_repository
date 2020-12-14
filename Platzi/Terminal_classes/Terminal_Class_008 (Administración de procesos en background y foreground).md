# Administración de procesos en background y foreground

### tipos de proccesos 	

- Foreground
> son procesos en primer plano y al ejecutarse en la consola no se puede escribir ni usar la consola en lo que termina de ejecutarse el proceso
- Background
> son procesos ejecutados en segundo plano y al utilizar el simbolo:
> 
**Amperesand**
```
&
```

>al final de la linea le podemos asignar el valor de segundo plano a nuestros comandos dentro de la terminal

Cualquier comando ya ejecutado se puede mandar a background con la combinación de teclas dentro de la terminal:

> Ctrl + z

*nota: los comandos mandados a background con ctrl + z no se continuan ejecutando hasta que los vuelves a traer a foreground a diferencia de con ampersand (&).*

Y si se quiere volver a mandar a foreground se utliziaría el
comando: 
```
fg
```
### Identificar procesos en segundo plano

**Herramientas:**
```terminal
ps
```
>Este comando muestra los procesos que yo estoy ejecutando
```terminal
ps -ax 
```
>Este comando muestra todos los procesos en segundo plano
```terminal
top
```
>Me muestra todos los procesos que se están ejecutando pero de manera interactiva y a comparación de ps, top me deja finalizar procesos

### Eliminar procesos en primer plano:

> Ctrl + c

### Salir de la terminal

> Ctrl + d


### Eliminar procesos en segundo plano:

Al ver nuestros procesos en segundo plano con:
```terminal
top
```
En el inicio de la linea de cada proceso viene un numero que es el PID (Priority_ID) o numero de prioridad, ese es el numero que utilizamos para identificar nuestro proceso

```terminal
kill

```
>Este comando envía señales a los procesos para que se detengan
>
>*nota: Con este comando no se interrumpen violentamente, puede terminar lo que está haciendo el proceso y luego eliminarse

```terminal
kill -9 <numero_de_proceso>
```
Termina todos los procesos que no puedas terminar con kill de una manera mas forzada.
*nota: Se pueden llegar a corromper los datos por cerrarlos de manera forzada así que solo se recomienda en casos donde el comando kill no funciona.*

```terminal
killall
```
Hace lo mismo pero en lugar de terminar por numero de proceso lo hace por el nombre del archivo ejecutable que esté disparando el proceso.