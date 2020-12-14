# Sistemas de manejo de paquetes

Sitema de manejos de paquetes te ayuda a gestiónar los paquetes que se desa instalar, se puede decir que es el vinculo entre tu queriendo ejecutar el paquete y el sistema de paquetes buscando y trayendo el paquete hasta ti para instalarlo

```
sudo apt-get update
```
> Mantiene tu lista de paquetes actualizada

```
sudo apt-get upgrade
```

```
sudo apt-get install
```
> Instalar


Importante: podemos instalar cualquier programa que esté disponible en los repositorios de Ubuntu, pero no podremos lanzar aquellos que hagan uso de una GUI, como Firefox (aunque no tendría sentido instalar nada que esté disponible para Windows de manera oficial)


las rutas. No son lo mismo y no las reconoce igual. El problema está en cómo las escribe Windows y cómo las necesita Linux. Lo bueno es que es fácil recordar cómo convertir una ruta de Windows a Linux.

Por ejemplo: la ruta C:\Users\Pablo\Destktop\ de Windows sería /mnt/c/Users/Pablo/Desktop. Sabiéndolo, si alguna vez queremos arrastrar un archivo de Windows al terminal de Ubuntu, lo que tenemos que hacer es básicamente cambiar las barras invertidas por barras normales, poner la «c» minúscula, quitar los dos puntos y delante añadir «/mnt/». No es difícil de recordar.