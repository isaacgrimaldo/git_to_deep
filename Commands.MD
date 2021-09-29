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

> Modifica el anterior commit 

`
 git reset --soft  HEAD^
`


# Manejo de Ramas

> Ver todas las ramas existentes 

`
  git branch
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
 
> Borra algun cambio hecho 

` 
 git reset [nameFile]  o git reset .
`

> para especifícar los tipos de docuemtos quieres agregar

`
  git add  [path +  * extencion(.js .html .css ...etc) ]  
`

