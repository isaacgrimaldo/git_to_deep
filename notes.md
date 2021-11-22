# Notas del Curso

-  cuando se quire agregar una carpeta sin ningun contenido, se le agrega un documento llamdo  .gitkeep para que git le de seguiento 


<hr>

- los alias son script que ayudan a aagilzar el trabajo 
  
   > Aqui unos de los que más uso

    1.  ` git config  --global alias.s 'status --short' `

    2. `git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all" `

<hr>

- Una forma de modificar un commit para agregar algun cambio extra, pero no hacer un commit extras se puede hacer la siguientemanera 

`  
  git reset --soft  HEAD^
`

> esto para el cambiar el primer commit, pero si se quiere hacer un commit desde un commit más anterior se hace de las siguien te manera

`
  git reset --soft  HEAD^[CommitNumber] 
`

> uso:   

`
git reset --soft  HEAD^[CommitNumber] (1, 2, 3 ...etc) 
` 

 #### Pero tiene su riesgo de perder informacion guardada

<hr>

 - el uso del git reset --mixed: Este comando se usa para viajar entre commit borrando los cambio del staged pero no de la carpeta, asi que, un te permite añandir 

`
  git reset --mixed [commitID] o HEAD^ 
`

<hr>

 - el uso del git reset --hard: Este comando se usa para viajar entre commits igual qur los dos anteriores, pero este vuele el estado del proyecto del commit al que viajo, borrandos todo los cambios nuevos

`
  git reset --hard [commitID] o HEAD^ 
`

<hr>

- ### Combinacion de ramas modo: fast-forward :
> esta forma de combinacion de rama es la mejor, ya que todo se hacer de manera automatica al ejecutar 
>  el commando: 

`
  git merge [mixRama]
`
 ### Recuerda que si quieres traer cambios de una rama a otra tienes que estar en la rama que quires traer 
 ### los cambios  y ejecutar el comando: `git merge [mixRama]`  para traer los cambio de la otra rama   


<hr>

## Notas sobre  los tags

 - los tags sirver puntos especificos de nuestro programas y poder identificarlos rapidamente 
 - se puden crear en forma semantica de verciones v[versionActual].[funcionalidadAñadida].[bugresuelto] 


## Notas sobre el stash
  
  - El stash solo en una forma de guarda avances rapidamente, no es muy recomendable trabajar con el 
 
## Rebase 

- lo rebase se usan para mover commit atravez del tiempo ya sea para combinarlos o modificarlos 
- para hacer rebase con una rama tienes que estar parado en la rama donde quieres que los commit sea modificados y correr el comando git rebase [name] de la rama a la que va dirijida el rebase  

### Rebase interactivo 

- esta forma de hacer rebase es mas funcional que la rebase normal. tiene un menu con multiples opciones para trabajar con los commit realizados  

- dentro de las funciones que se pueden realizar con un rebase interactivo estan 
  * cambiar el mensaje del commit 
  * combinar commits 
  * borrar commits
  * editar commits