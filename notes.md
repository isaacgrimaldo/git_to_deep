# Notas del Curso

-  cuando se quire agregar una carpeta sin ningun contenido, se le agrega un documento llamdo  .gitkeep para que git le de seguiento 



- los alias son script que ayudan a aagilzar el trabajo 
  
   > Aqui unos de los que más uso

    1.  ` git config  --global alias.s 'status --short' `

    2. `git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all" `

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

 ### Pero tiene su riesgo de perder informacion guardada
