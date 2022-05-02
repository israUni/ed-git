# Etiquetas en GIT  

Las etiquetas *tags* nos ayudan para establecer una marca en un determinado punto de nuestro proyecto.  

Listar etiquetas creadas en orden alfabético:  
`git tag`

## Etiquetas  

### Etiquetas "ligeras"  
Es un *"checksum"* de un commit guardado en un archivo, no incluye más información. Para la creación de estas etiquetas no es necesario agregar las opciones: `-a`, `-s`, ni `-m`.  
Agregar una etiqueta a nuestro último commit ->(Se pueden agreagar etiquetas a cualquier commit)
`git tag <tagName> -dev`

Agregar una etiqueta en algun punto de nuestro proyecto:  
`git tag <tagName> <commitHash>`

### Etiquetas "anotadas"  
se guardan en la base de datos de GIT como objetos enteros. Tienen un *checksum*; contienen el nombre del etiquetador, correo, fecha y un mensaje asociado.  
`git tag -a <tagName> -m "Project Version 1.0.0"`

Ver una etiqueta en específico:  
`git show tagName`  

### Filtrado de etiquetas  
