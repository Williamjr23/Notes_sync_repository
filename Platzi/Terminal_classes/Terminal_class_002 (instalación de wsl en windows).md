# instalación de wsl en windows

Para acceder a la terminal de Linux desde windows se necesita instalar la distribución de "windows subsystem for Linux"

Una vez instalado se podrá colocar cualquier distribución de Linux

Con acceso de administrador a la PC abres **Windows PowerShell**

Una vez allí escribe el siguiente comando:

```PowerShell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux.
``` 

Y reinicia el ordenador

Luego en la microsoft store busca tu versión favorita de linux #ubuntu 20.4 lts

Al lanzar tu terminal ingresa tu nombre de usuario #puede ser distinto al de windows

Y crea tu contraseña

Y listo ya tienes una terminal linux dentro de tu windows 

Un último detalle importante

>los archivos que tienes en tu Linux le pertenecen… Para acceder a los archivos que tienes en Windows (o grabar nuevos archivos desde tu Linux) debes ingresar en

```dir
/mnt/c/Users/"TU_USUARIO"
```

>donde TU_USUARIO debe ser reemplazado por tu nombre de usuario de Windows.

Ahora sí, cualquier archivo que guardes en esa localización podrá ser accedido con las herramientas propias de Windows.