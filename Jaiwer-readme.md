# Notas personales de Jaiwer Castillo

## Comandos aprendidos

#### Git init. Con git init inicias un repositorio para poder trabajar con git. Ejemplo:
```Shell 
git init
```

#### Luego de haber iniciado con "git init" viene la iteración básica. 


#### Git status. Te permite ver el estado de los archivos del repo. Si haces algun cambio y quieres estar seguro si se completó, basta con colocar este comando y te muestra: 
```Shell
git status
```
#### Git add. Se usa para agregar cambios al staging área. Hay diferentes formas de usar el "git add". Ejemplo: 
```Shell
git add [nombre del archivo]. Agrega el cambio o creación del archivo de manera individual.

git add -A. Agrega los cambios de todos los archivos creados. 

git add [nombre de archivo]/[nombre de archivo]/[nombre de archivo]. Agrega varios cambios a la vez.
```
#### Git commit. Inserta los archivos que se encuentren en el staging área y los coloca en el repositorio. El "git add" junto al "git commit" se define como el proceso básico de GIT. Hay diferentes formas de usar el "git commit". Ejemplo:
```Shell 
git commit -m "nombre del título de commit". 

git commit --amend. Corrige el commit mas reciente.
```

#### Git clone. Crea una copia de un repositorio existente en tu terminal. Clonar es el camino más común para obtener una copia de un proyecto. Git clone se usa así: 
```Shell
git clone [Dirección del repositorio]
```
#### Git checkout. Te permite mover entre commits y archivos, git checkout también te permite moverte entre ramas.

#### Para usarlo entre commits es:
```Shell
git checkout [ID del commit]
```
#### Para usarlo entre ramas es:
```Shell
git checkout [nombre de la rama]
```
#### Git branch. Te permite crear una rama nueva. Una vez creada, debes ubicarte en ella para comenzar a trabajar en tu nueva rama. Su iteración es: 

#### Para crear la rama:
```Shell 
git branch [nombre de la rama a crear]
```

#### Para moverte hacia ella:
```Shell
git checkout [nombre de la rama creada]  
```

#### Git log. Te ayuda a explorar las previas revisiones de un proyecto: 
```Shell 
git log
```

#### Git alias. Es un comando que te permite crear tus propios comandos de GIT a partir de otros. Este comando a continuación te permite ver "git log" de una manera más dinámico, aparte de que ayuda mucho a la hora de usar "git log":
```Shell
git config --global alias.superlog "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
```

#### Git merge. Fusiona, permite integrar cambios de ramas diferentes en una sola: 
```Shell
git merge branch1/branch2
```
#### Git pull. Es la versión automática de git fetch. Descarga la rama desde un repositorio remoto y luego lo fusiona con la rama actual.
```Shell 
git fetch + git merge = git pull
```
#### Git push. Te permite mover una rama local a otro repositorio, usualmente es la forma de publicar las contribuciones en un servidor remoto.
```Shell
git push [nombre del remoto] [nombre de la rama]
```
#### Git remote. Te permite conectar repositorios locales y remotos. Sirve para que en lugar de poner la URL para realizar "fetch o pull", solo le asignaremos un nombre y así podremos llamar a esa conexión de manera rápida. Por defecto se llama "origin".
```Shell 
git remote add [nombre del remoto]
```
--------------------------------------------------------

***[Volver al inicio](Jaiwer-readme.md)*** 

--------------------------------------------------------

***[Regresar al archivo README](README.md)***

--------------------------------------------------------