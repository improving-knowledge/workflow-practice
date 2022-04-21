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
```Shell
git log
git log --name-status
```
#### El comando git init se utiliza para iniciar git. Crea una zona llamada staging dentro de la memoria RAM donde se irán guardando los cambios que se hagan sobre el archivo. Ejemplo:
```Shell
git init
```
#### Para iniciar GIT en la carpeta donde esta el proyecto (Se usa una sola vez). Ejemplo:
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

--------------------------------------------

## Estructura de los Mensajes en los COMMITS

Al crear un commit luego de añadir los archivos modificados/creados
y estas por agregar informacion sobre lo que hiciste, lo mas práctico
es escribir unas pocas palabras para informar sobre el cambio.
Ej.
```Shell
git commit -am "Agregue la funcion eliminar"
```
Pero, en proyectos mas grandes y complejos, es mejor utilizar los
estandares propuestos. Ej.
```Shell
git commit
```
Ustedes dirán  "y donde está el mensaje?". Pués al ejecutar el commit
de esa manera, sin parametros ni nada, les abrirá un editor donde
colocar una descripcion mas amplia de lo que hicieron. La siguiente
documentacion explica la forma de escribir la informacion del commit
de una forma más detallada y explicita:

- El mensaje de un commit consiste en 3 diferentes partes
separadas por una linea en blanco: el titulo, un cuerpo
opcional y un pie opcional. Algo como lo siguiente:

-------------

type: subject

body

footer

-------------

El titulo consiste en el tipo y asunto del mensaje.
Type / Tipo

El asunto no debe contener mas de 50 caracteres,
debe iniciar con una letra mayuscula y no terminar con un punto.
El tipo es contenido en el titulo y puede ser de alguno de los siguientes casos:

- feat: Una nueva caracteristica
- fix: Se soluciono un bug
- docs: Se realizaron cambios en la documentacion
- style: Se aplico formato, comas y puntos faltantes, etc; Sin cambios en el codigo
- refactor: Refactorizacion del codigo en produccion
- perf: Un cambio en el código que mejora el desempeño
- test: Se añadieron pruebas, refactorizacion de pruebas; Sin cambios en el codigo
- chore: Actualizacion de tareas de build, configuracion del admin. de paquetes; sin cambios en el codigo

Al escribir el cuerpo (Body), requerimos de una linea en blanco
entre el titulo y el cuerpo, ademas debemos limitar la longitud
de cada linea a no mas de 72 caracteres.

El pie es opcional al igual que el cuerpo, pero este es usado
para el seguimiento de los IDs con incidencias. Ej:

Resolve: #6113
Closes: #456, #789, #45

Plantilla ejemplo:

--------------------------------------------------------

feat: Ultima documentacion del Readme

Se agregaron comandos para solucionar conflictos <br />
ademas de la informacion sobre las plantillas de <br />
los mensajes largos en los commit

Resolve: #123

--------------------------------------------------------

***[Contribucion de Jaimar Angulo](jaimarkas-readme.md)***

--------------------------------------------------------

***[Notas personales de Bresmar Bermudez](Bresmar-readme.md)***

--------------------------------------------------------

***[Notas personales de Jaiwer Castillo](Jaiwer_README.md)***

--------------------------------------------------------

