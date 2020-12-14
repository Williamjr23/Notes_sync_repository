# Instalando Git y GitBash en Windows

### si tienes ubuntu o devian:
```terminal
apt-get install git
```
nota: se recomienda hacer un 
```terminal
apt upgrade
```
y un 
```terminal
apt update 
```
antes de instalar 

### Instalando Git (desde 0)

**1. Descargar e instalar git:**
Entrar a [**git**](https://git-scm.com/) y descargar la version deseada

**2. Instalar git**

Ejecutar la instalación como normalmente y asegurarte de marcar la casilla:

- [x] Get Bash Here

Unas cuantas opciones despues nos preguntará si usamos solo el editor de Git bash o también podremos introducir comandos de git en terminales de terceros, en este caso preferiremos la segunda opción:

- [x] Get from the command line and also from 3rd-party software

Despues elegiremos que tipo de librería se va a usar para la seguridad, la primera opción es para conectarte con llaves ssh entre otras que no están pre instaladas en windows y la segunda es solo para las que tiene windows por defecto en este caso seleccionaremos la segunda opción

- [x] Use the OpenSSL library

Después nos pregunta sobre la configuración conversion de terminado de lineas en la cual la primera opción es la mas compatible entre todos o la mas global:

- [x] Checkout Windows-style, commit Unix-style line endings
>Se reciven los saltos en linea de la manera en windows y al enviarse se convierten en la manera de linux o unix
- [ ] Checkout as-is, commit Unix-style line endings
>En esta opción es como esté especificado en el sistema de windows
- [ ] checkout as-is, commit as-is
>No se hacen conversiones

Luego pregunta si quieres usar cmd o su propio sistema de emulacion MinTTY en este caso seleccionaremos:

- [x] Use MinTTY (The default terminal of MSYS2)

- [ ] Use windows'default console window 

Y daremos instal y terminó la instalación de git

