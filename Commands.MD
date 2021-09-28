# GIT Commands   

## Comandos de configuración  

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



## Comandos Generales de Git

> Crean un nuevo repositorio 

`
   git init
`

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

> Guarda los cambio en un commit con algun pequeños mensaje para decir lo que cambio

`
 git commit -m '[descripcion]'
`

> Añadir los los cambios y Guardarlos con un commmit al mismo tiempo (Solo funciona con documentos que esten en seguimiento pot git)

`
 git commit am  ['commit']
`

> Regresa el proyecto al ultimo commit hecho 

`
 git checkout -- . 
`

> Ver commit realizados

`
 git log
`

## Manejo de Ramas

> Ver todas las ramas existentes 

`
  git branch
`

> Cambiar el el nombre de una rama 

`
 git branch  -m [nameBranch] [newNameBranch]
`