# workflow-practice
> Repositorio de prácticas para el flujo de trabajo en Github. Superplus3

## Comandos GIT importantes:

#### Para descargar un repositorio desde un servidor remoto. Ejemplo: Github.
```Shell
git clone git@github.com:pulidovpe/practica_workflow.git
```
#### Muestra la lista de los archivos que se han cambiado junto con los archivos que están por ser preparados o confirmados. Ejemplo:
```Shell
git status
```
#### Para agregar un nuevo archivo o uno modificado. Ejemplo:
```Shell
git add archivo.txt
```
#### Para agregar varios archivos. Ejemplo:
```Shell
git add archivo.txt carpeta/otro_archivo.txt otra_carpeta/otro_archivo.txt
```
#### Para agregar todos los archivos del proyecto. Ejemplo:
```Shell
git add -A
git add --all
```
#### Permite ver la informacion de los cambios hechos. Ejemplo:
``Shell
git log
git log --name-status
```
#### Para iniciar GIT en la carpeta donde esta el proyecto. Se usa una sola vez Ejemplo:
```Shell
git init
```
#### Para confirmar la instantánea preparada en el proyecto mediante un mensaje de confirmación. Ejemplo:
```Shell
git commit
```
#### Para cargar en el HEAD los cambios realizados y establecer el mensaje del commit. Ejemplo:
```ssh
git commit -m "Texto que identifique por que se hizo el commit"
git commit -m "Modificando archivo README.md"
```
#### Agregar y Cargar en el HEAD los cambios realizados. El parametro `-a o --all` confirma todos los archivos en el área de trabajo (esos nuevos, con modificaciones, o incluso eliminados) automáticamente. Ejemplo:
```ssh
git commit -a -m "Texto que identifique por que se hizo el commit"
git commit -a -m "Modificando archivo README.md"
```
#### Para ver conflictos (de haberlos). Ejemplo:
```ssh
git commit -a
```
#### Para reescribir el último commit con cualquier cambio que esté en el área de preparación o un nuevo mensaje. Ejemplo:
```ssh
git commit --amend -m "Texto que identifique por que se hizo el commit"
git commit --amend -m "Mejorando la lista de comandos git"
```
