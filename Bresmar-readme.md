<a name="#inicio"></a>

#### Inicio

## Indice de Contenido
| ***[COMANDOS PARA LA INTERACCION BASICA](#comandos-para-la-interacción-básica)*** |
| ***[CONFIGURACIÓN BASICA](#configuración-básica)*** |
| ***[OTROS COMANDOS](#otros-comandos)*** |
| ***[¿QUÉ ES UN PULL REQUEST?](#qué-es-un-pull-request-)*** |
| ***[¿CUALES SON SUS PASOS?](#cuales-son-sus-pasos)*** |
| ***[¿QUÉ SON LOS MILESTONES?](#qué-son-los-milestones-)*** |


## **Notas personales de: Bresmar Bermúdez**: 📌
>*Comandos aprendidos en el curso de Git y Github*

<a name="#comandos-para-la-interacción-básica"></a>
## **COMANDOS PARA LA INTERACCIÓN BÁSICA**:

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
***[Volver al inicio](#inicio)***

<a name="#configuración-básica"></a>
## **CONFIGURACIÓN BÁSICA:**

#### Configurar el nombre que sale en los commits. Ejemplo:
```Shell
git config --global user.name "Bresmar Cortez"
```
#### Configurar Email. Ejemplo:
```Shell
git config --global user.email Bresmarcortez@gmail.com
```

<a name="#otros-comandos"></a>
## **OTROS COMANDOS:**

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
***[Volver al inicio](#inicio)***

<a name="#qué-es-un-pull-request-"></a>

----------------------------------------------------------------------------------
## ¿Qué es un ***Pull Request***? 📌

```Shell
Un pull request es una petición que el propietario de un fork de un repositorio hace al propietario del repositorio original para que este último incorpore los commits que están en el fork. En el caso que nos ocupa, el usuario `Bresmar` le enviará la petición a la organización `aprendiendo-github` para que este último incorpore los commits que tiene en su fork.
```
<a name="#cuales-son-sus-pasos"></a>

### ¿Cuales son sus pasos?
Para hacer un pull request se deben seguir los siguientes pasos:
```Shell
1. Ve a tu cuenta de GitHub y selecciona el repositorio donde deseas hacer la petición.
2. Verás un botón llamado "Pull request", has clic en él.
3. Presiona "New pull request" para crear el nuevo pull request
4. Has clic en el boton "Create pull request"
5. Colocale un titulo y una descripción en las areas correspondientes para generar el comentario.
6. Vuelve hacer clic en "Create pull request" para finalizar y esperar ser evaluado por el responsable del proyecto, quien decide si se aceptan tus cambios (commits) o no.
```

<a name="#qué-son-los-milestones-"></a>

## ¡Bono Extra!...¿Que son los Milestones? 🎁
```Shell
Son una manera de agupar issues en categorias para filtrar mejor la información
```
***[Volver al inicio](#inicio)***

--------------------------------------------------

***[Volver al archivo README](README.md)***
--------------------------------------------------
