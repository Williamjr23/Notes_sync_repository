# Tratamiento de texto

## trabajo fundamental con archivos de texto:
Nos permite crear nuevos archivos:
>```Terminal
>touch
>```
>Ejemplo:
>```Terminal
>touch archivo.txt
>```


Nos permite visualizar todo el contenido de nuestros archivos:
>```Terminal
>cat
>```
>Ejemplo:
>```Terminal
>cat archivo.txt
>```

También nos permite visualizar el contenido de nuestros archivos, debemos indicarle cuántas líneas nos debe mostrar. Por defecto nos mostrará las primeras 10.
>```Terminal
>head
>```
>Ejemplo:
>```Terminal
>head -n 20 archivo.txt
>```
>nota: **-n <numero de lineas a mostrar>** es indicar el numero de lineas a mostrar
>
>Ejemplo:
>```Terminal
>-n 20
>```

Funciona igual que el comando head pero al revés y tambien se indica el numero de lineas a mostrar:
>```Terminal
>tail
>```
>Ejemplo:
>```Terminal
>tail -n 20 archivo.txt
>```

## Busqueda y tratamiendo de texto: