# Manejo de ramas (branches)  

## Creación de ramas  
`git branch <branchName>`

## Desplegar listas de las ramas de nuestro proyecto  
`git branch`

## Moverse a determinada rama  
`git checkout <branchName>`

## Visualización de las ramas
`git log --all --graph`

## Fusión/mezcla/unificación de ramas  
`git merge <branchNameToMerge>`

Esta linea se creó en la rama: firstBranch, pero servirá de ejemplo en la unión de la rama firstBranch a la rama principal main. NOTA: Para ello tenemos que "movernos" a la rama main...  

Ahora "eliminaremos" la rama firstBranch, esto lo podemos hacer ya que la rama firstBranch se fusionó/unió a la rama principal (main)  
`git branch -d <branchName>`  

En caso de necesitemos eliminar una rama aunque esta no haya sido unificada, entonces utilizaremos el siguiente comando:
`git branch -D <branchName>`  
Con la opción `-D`, forzaremos a la eliminación de la rama requerida, por lo que es altamente recomendable utilizarse siempre y cuando estemos 100% seguros que es lo que realmente queremo/necesitamos hacer...