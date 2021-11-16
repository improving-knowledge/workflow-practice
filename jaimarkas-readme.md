Notas personales de Jaimar Angulo

Comandos en Git

#### Para ver la version de git. Ejemplo:
```Shell
git version
```
#### Para ver solo el commit con el nombre. Ejemplo:
```Shell
git log --oneline
```
#### Para copiar un repositorio. Ejemplo:
```Shell
git clone <url>
```
#### Para subir al repositorio. Ejemplo:
```Shell
git push origin master
```
#### Para reeditar el ultimo commit. Ejemplo:
```Shell
git commit --amend -m "Texto que identifique porque se hizo el commit "
```

GIT HEAD

#### Saca un archivo del commit. Ejemplo:
```Shell
git reset Head <Archivo>
```
#### Devuelve el ultimo commit que se hizo y pone los cambios en staging. Ejemplo:
```Shell
git reset --soft HEAD^
```
#### Devuelve el ultimo commit y todos los cambios. Ejemplo:
```Shell
git reset --hard HEAD^
```
#### Devuelve los 2 ultimo commit y todos los cambios. Ejemplo:
```Shell
git reset --hard HEAD^^
```


GIT REMOTE

#### Agregar repositorio remoto. Ejemplo:
```Shell
git remote add origin <url>
```
#### Cambiar de remote. Ejemplo:
```Shell
git remote set-url origin <url>
```
#### Remover repositorio. Ejemplo:
```Shell
git remote rm <name/origin>
```
#### Muestra lista repositorios. Ejemplo:
```Shell
git remote -v
```
#### Muestra los branches remotos. Ejemplo:
```Shell
git remote show origin
```
#### Limpiar todos los branches eliminados. Ejemplo:
```Shell
git remote prune origin
```


GIT BRANCH

#### Crea un branch. Ejemplo:
```Shell
git branch <nameBranch>
```
#### Lista los branches. Ejemplo:
```Shell
git branch
```
#### Elimina el branch y lo une al master. Ejemplo:
```Shell
git branch -d <nameBranch>
```
#### Elimina sin preguntar. Ejemplo:
```Shell
git branch -D <nameBranch>
```


GIT TAG

#### Muestra la lista de todos los tags. Ejemplo:
```Shell
git tag
```

#### Crea un nuevo tag. Ejemplo:
```Shell
git tag -a <version> -m "esta es la version x"
```
GIT REBASE
Los rebase se usan cuando trabajamos con branches esto hace que los branches se pongan al dia con el master sin afectar al mismo.


#### Une el branch actual con el master, esto no se puede ver como un merge. Ejemplo:
```Shell
git rebase
```
#### Cuando se produce un conflicto nos da las siguientes opciones: Cuando resolvemos los conflictos --continue continua la secuencia del rebase donde se pauso. Ejemplo:
```Shell
git rebase --continue
```
#### Omite el conflicto y sigue su camino. Ejemplo:
```Shell
git rebase --skip
```
#### Devuelve todo al principio del rebase
```Shell
git rebase --abort
```
#### Para hacer un rebase a un branch en especifico. Ejemplo:
```Shell
git rebase <nameBranch>
```


OTROS COMANDOS

#### Lista un estado actual del repositorio con lista de archivos modificados o agregados. Ejemplo:
```Shell
git status
```
#### Quita del HEAD un archivo y le pone el estado de no trabajado. Ejemplo:
```Shell
git checkout -- <file>
```
#### Une el branch actual con el master, esto no se puede ver como un merge. Ejemplo:
```Shell
git rebase
```
#### Crea un branch en base a uno oneline. Ejemplo:
```Shell
git checkout -b newlocalbranchname origin/branch-name
```
#### Busca los cambios nuevos y actualiza el repositorio. Ejemplo:
```Shell
git pull
```
#### Cambiar de branch. Ejemplo:
```Shell
git checkout <nameBranch/tagname>
```
#### Une el branch actual con el especificado. Ejemplo:
```Shell
git merge <nameBranch>
```
#### Verifica cambios en el repositorio oneline con el local. Ejemplo:
```Shell
git fetch
```
#### Borrar un archivo del repositorio. Ejemplo:
```Shell
git rm <archivo>
```
