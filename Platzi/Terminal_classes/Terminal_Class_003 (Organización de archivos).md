# Organización de archivos

Reglas

- No pueden existir en un mismo directorio con el mismo nombre
- No pueden contener caracteres especiales
- no dejar espacios nunca en nombres de carpetas

Comandos moverse entre carpetas:

```terminal
.. #directorio padre

. #directorio actual

cat #concatena archivos y los muestra

man #se antepone ante cualquier comando y significa manual

cd ~ #Lleva directamente a /home

cd - #Lleva al ultimo directorio visitado

ls #Listar archivos

ls -a #Listar archivos ocultos

ls -l #Muestra toda la información: usuario, grupo, permisos, tamaño, fecha y hora de creación.

ls -lh #Muestra la misma información que ls -l pero con las unidades de tamaño en KB, MB:

pwd #Identificar directorio

cd #Cambiar de directorio

mkdir #Crear un directorio

cp #Copiar un archivo

rm #Borrar un archivo

mv #Mover un archivo

#Ejemplo
mv introduccion_linux /home/crinto/learning/
#

rmdir #eliminar un directorio
```