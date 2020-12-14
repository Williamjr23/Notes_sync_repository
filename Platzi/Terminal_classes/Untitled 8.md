# Terminal class 009  (Permisos sobre archivos sistema octal)

### sistema de permisos octal:
Esto se llama notación octal porque los números binarios se convierten a base 8 utilizando los dígitos del 0 al 8:

### Usuarios:

- Dueño (Quién creó el archivo)
- Grupo (Con quien se comparte el archivo)
- Otros (Que se les permite hacer a los otros usuaros ajenos)

### Tabla de permisos:
Esta es una tabla de permisos que aplica para los 3 tipos de usuarios:

|  r  |  w  |  x  |     |
|:---:|:---:|:---:|:---:|
|  1  |  0  |  0  |  4  |
|  1  |  1  |  0  |  6  |
|  1  |  1  |  1  |  7  |

Arriba en la tabla podemos ver los 3 tipos de permisos que se pueden otorgar a cada usuario los cuales son:

- Lectura (**R**ead)
- Escritura (**W**rite)
- Ejecución (e**X**ecution)
> nota: eXecutión o X en carpetas significa que el usuario tiene acceso, mientras que en programas significa que el usuario tiene permiso para ejecutarlo

En la parte de abajo, cada casilla tiene un valor 0 o 1 , que representa si el permiso está otorgado (1) o no lo está (0) y al final de cada fila viene la representación de el numero que forma el conjunto de permitido o denegado de cada uno de los 3 permisos

Ejemplo:

| sistema binario | sistema decimal |
|:---------------:|:---------------:|
|       100       |        4        |
|       110       |        6        |
|       111       |        7        |

Entonces los permisos en la terminal se ven de la siguiente manera:

>Este sería uno de los comandos que se pueden introducir para conocer los permisos:
>```termial
>william@DESKTOP-L11ITB8:~/Platzi_Terminal$ ls -l
>```

>Esto sería lo que nos arrojará la terminal:
>```terminal
>total 20
>drwxrwxr-x 2 william william 4096 Nov 23 15:59 Personal_Projects
>drwxr-xr-x 2 william william 4096 Nov 16 22:36 Terminal_003
>drwxr-xr-x 2 william william 4096 Nov 17 17:30 Terminal_005
>drwxr-xr-x 2 william william 4096 Nov 21 20:09 Terminal_007
>drwxr-xr-x 2 william william 4096 Nov 23 16:55 Terminal_009
>william@DESKTOP-L11ITB8:~/Platzi_Terminal$
>```

Como podemos ver entonces las letras que aparecen al principio de cada archivo corresponde a los permisos:

>drwxrwxr-x

detalle:
- d : directory
- r : Read
- w : Write
- x : eXecution
- \- : Permiso denegado

Despues de la **d** se divide en 3 partes: / rwx / rwx / r-x /

- Primera:corresponde al dueño
- Segunda:Corresponde al grupo
- Tercera:Corresponde a otros

### Modificar los permisos manera octal:

Comos su nombre lo indica esta manera de cambiar los permisos se basa en la tabla que vimos anteriormente y es la forma mas eficiente de cambiar los permisos ya que ahorras tiempo y otorgas varios permisos a la vez

comando: 
```terminal
chmod
```
utilidad:
>este comando nos sirve para cambiar los permisos de un archivo o carpeta, y sus opciones
nos permiten cambiar los permisos también sobre los subdirectorios entre otros...

Opciones:
```terminal
 --help
```
>Muestra la ventana de otras opciones del comando no mencionadas aquí
```terminal
-R
```
>Significa "Recursive" y su función es hacer que este funcione también tomando en cuenta
los subdirectorios de la ruta

```terminal
-v
```
>Su output es mostrar todos los ficheros procesados en la ejecución de cambio de permisos 

```terminal
-c 
```
>Es como -v, pero solo avisa de los ficheros a los que se modificaron sus permisos

sintaxis:
```terminal
chmod [opciones] [permisos_a_3_digitos] [archivo.txt_o_directorio/]
```
Ejemplo:
```terminal
chmod -R -v 740 direcotorio/
```

comando: 
```terminal
chown
```
utilidad:
>este comando nos sirve para cambiar el dueño de un archivo o carpeta

Opciones:
>mismas opciones que en chmod

sintaxis:
```terminal
chown [opciones] [Dueño] [archivo.txt_o_directorio/]
```
Ejemplo:
```terminal
chown -R -c root /var/home
```
comando: 
```terminal
chgrp
```
utilidad:
>Se utiliza para cambiar el grupo al que pertenece un archivo o directorio.

Opciones:
>mismas opciones que en chmod y chown

sintaxis:
```terminal
chown [opciones] [Grupo] [archivo.txt_o_directorio/]
```
Ejemplo:
```terminal
chgrp -R -c grupo_nuevo algo.txt
```
Superuserdo (sudo)

```terminal
sudo
```

se ejecuta anteponiendose a otros comandos para correr en modo administrador