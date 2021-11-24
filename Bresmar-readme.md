### **Notas personales de: Bresmar Bermúdez**:
>*Comandos aprendidos en el curso de Git y Github*

**COMANDOS PARA LA INTERACCIÓN BÁSICA**:

#### Agregar un archivo a ser preparado para un commit. Ejemplo:
```Shell
git add <Nombre del archivo>
git add index.html
```
#### Agregar todos los archivos con cambios para un commit. Ejemplo:
```Shell
git add -A
```
#### Cargar en el HEAD los cambios realizados. Ejemplo:
```Shell
git commit -m "texto relacionado con el cambio registrado"
git commit -m "Archivo index.html modificado"
```
#### Ver el estado del repositorio con una lista de archivos cambiados o agregados. Ejemplo:
```Shell
git status
```

**CONFIGURACIÓN BÁSICA:**

#### Configurar el nombre que sale en los commits. Ejemplo:
```Shell
git config --global user.name "Bresmar Cortez"
```
#### Configurar Email. Ejemplo:
```Shell
git config --global user.email Bresmarcortez@gmail.com
```

**OTROS COMANDOS:**

#### Ver el historial de los commit hechos. Ejemplo:
```Shell
git log
git log --oneline
git log --oneline --graph
```
#### Borrar un commit (se borrará todo desde el id del commit selccionado para arriba). Ejemplo:
```Shell
git reset --hard <id del commit>
git reset --hard 0beefde
```
#### Crear ramas. Ejemplo:
```Shell
git branch <Nombre de la rama>
git branch Pokmont
```
#### Ver una lista de las ramas creadas. Ejemplo:
```Shell
git branch
```
#### Para desplazarte entre las ramas creadas. Ejemplo:
```Shell
git checkout <Nombre de la rama a donde se desea desplazar>
git checkout Pokmont  
```
#### Borrar una rama. Ejemplo:
```Shell
git branch -d <Nombre de la rama>
git branch -d Pokmont
```
#### Hacer fusion. Ejemplo:
```Shell
git merge <Rama que se desea fusionar>
git merge pokmont
```
#### Para clonar o copiar un repositorio. Ejemplo:
```Shell
git clone <URL del repositorio>
git clone  https://github.com/Bresmar/workflow-practice.git
```
#### Subir la rama master del proyecto local al repositorio remoto. Ejemplo:
```Shell
git push origin master
```
#### Bajar los cambios del repositorio remoto al proyecto local. Ejemplo:
```Shell
git pull
```
#### Observar la lista de remotos conectados. Ejemplo:
```Shell
git remote -v
```
#### Guardar los cambios temporalmente, para luego utilizarlos en cualquier rama. Ejemplo:
```Shell
git stash
```
#### Observar cambios en un archivo. Ejemplo:
```Shell
git diff
```
#### Verifica cambios en el repositorio online con el local. Ejemplo:
```Shell
git fetch
```
