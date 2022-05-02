## Subir repositorio a github.com

### Creación de cuenta en github.com
Es necesario accesar a https://githug.com y realizar el registro como mejor creamos conveniente.

### Creación de repositorio en github.com
- Dentro de nuestra cuenta de github.com, buscaremos la opción para crear un nuevo repositorio
- Asignar un nombre para identificar nuestro proyecto
- Opcional - agregar descripción
- Seleccionar la opcion de *Public*
- Pulsar boton de *Create repository*
- En nuestra terminal, corremos el siguiente comando: `git remote add origin https://github.com/<userName>/<repositoryName>`
- Con la actualización de Agosto de 2021, ahora debemos tener configurado el "Personal Access Token (PAT)", teniendo este token, ingresamos el siguiente comando en nuestra terminal: `git config user.password <enterAllYourPersonalAccessToken>`
- Ahora podemos correr el siguiente comando: `git push -u origin main` y se nos abrirá una ventana que nos pedirá el userName/email y posteriormente el password, en este caso ingresaremos el PAT para vincular git con github