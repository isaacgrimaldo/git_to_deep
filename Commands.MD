# GIT Commands   

# Comandos de configuración  

> Te muestras las configuraciones globales de git y te permite cambiarlas 

`
 git config --global -e  
`

 > Cambia los valores globales de un valor en específico

`
 git config --global [congif.types] [newValue] o ['newString']
`

> configura las rama creada por defecto 

`
 git config --global init.defaultBranch [name]
`
> para arreglar los warnings de LF would be replaced by CRLF en  windows usa los los siguentes comandos

`
  git config --global core.autocrlf false
`

`
  git config --global core.safecrlf true
`

> Creacion de alias para agilizar el trabajo

`
 git config --global alias.[aliasName] ['script']
`
> uso  :
`
  git [aliasName]
`


# Comandos Generales de Git

> Crean un nuevo repositorio 

`
   git init
`

> Guarda los cambio en un commit con algun pequeños mensaje para decir lo que cambio

`
 git commit -m '[descripcion]'
`

> Añadir los los cambios y Guardarlos con un commmit al mismo tiempo (Solo funciona con documentos que esten en seguimiento pot git)

`
 git commit -am  ['commit']
`

> Regresa el proyecto al ultimo commit hecho 

`
 git checkout -- . 
`

> Ver commits realizados

`
 git log
`

> Muestra las cambios realizados en un documento

`
 git dif (general) git diff [nameFile] (específica)
`

> Modifica el mensaje puesto en el ultimo commit para corregir algun error al haber lo hecho

`
git commit --amend -m ['newCommit']
`

> Muestra todo los log desde los inicio del tiempo (permite optner los [commitID])

`
 git  reflog
`


> Modifica el anterior commit  (sin borrar los cambios)

`
 git reset --soft  HEAD^
`

> Moifica puede ir a cualquier commit y segir desde ese punto (borra el steged pero no lo cambios ralizados)

`
  git reset --mixed  [commitID] o HEAD^ (para ir al anterior commit)
`

> Viaja a un commit en especifico y pudes trabajar desde ese punto ( Borra todo los cambios que no estan guardados en ese commit)

`
 git reset --hard [commitID] o HEAD^ (para ir al anterior commit)
`

# Manejo de Ramas

> Ver todas las ramas existentes y ver en la que te encuentras

`
  git branch
`

> Crear nueva ramaa

`
  git branch  [newNameRama]
`
> cambiar de rama 

`
  git checkout [nameRama]
`

> combinar rama 

`
  git merge [mixRama]
`

> Cambiar el nombre de una rama 

`
 git branch  -m [nameBranch] [newNameBranch]
`



# Manejo del staged 

> Muestra el estado de los cambio del repositorio

`
  git  status
`

> Añade los cambio hacea de forma automatica o  ingresando el paht del documento

`
  git add .   &&   git add [fileName] 
`
 
> Borra del staged todos los cambios hechos

` 
 git  reset .
`

> para especifícar los tipos de docuemtos quieres agregar

`
  git add  [path +  * extencion(.js .html .css ...etc) ]  
`

> Quita del stoged  los cambios hechos 

`
  git restore  .  o  git restore [fileName] 
`

<hr>

# Manejo de archivos

<br>

>  Cambia el nombre del documento

`
   git mv [fileName]  [newFileName]
 `

>  Borra docuentos sin contenido 

`
  git rm [fileName]
`

> Borra docuentos unque tengan contenido

`
 git rm -rf [filename]
`

<hr>

# Manejo de tags
 
> crear un tag de modo de versiones semantica  o solo por solo nombre de indetificación 

`
  git tag [nameTag]
`

> borrar un tag 

`
  git tag  -d [nameTag]
`

> crear un tag con una anotation en estado actual donde te encuentras en la aplicación 

`
  git tag  -a [nameTag] -m ['message']
`

> crear un tag con una anotation en un commit especifíco de la aplicación 

`
  git tag  -a [nameTag]  [hashCommit] -m ['message']
`

> te muestra toda la información detallada de un tag en especifíco

`
  git show [tagName]
`
