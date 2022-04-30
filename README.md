# Curso GIT por @EscuelaDigital

## Comandos de configuración iniciales básicos
```
git config --global user.name "Your Name Goes Here"
git config --global user.email "youremail@goeshere.com"
git config --global core.editor atom|subl|nano|code
git config --list
git config help <action>
git <action> --help

```

## Comandos básicos para el manejo de commits

```
git init // Iniciar git en nuestro proyecto
git add <filename> // Agregar un archivo/directorio al estado de seguimiento
git add . // Agregar todos los archivos al estado de seguimiento
git add -A // Agregar los archivo seguidos al estado de seguimiento
git status // Verificar el estado de los cambios
git commit // Abrir el editor de código configurado
git commit m- "Your descriptive commit description goes here"
git log // Verificar el historial de commits
git diff // Verificar las diferencias entre el directorio de trabajo y el directorio de preparación
git diff --staged // Verificar las diferencias en el directorio de preparación
git reset HEAD <fileName> // Saca un archivo del area de preparación y lo lleva al árbol de trabajo
git commit --amend // Reemplaza el último commit de la rama actual y tambien para agregar nuevos cambios a la utlima confirmación/commit realizado
git commit -a -m
git rm <fileName> // Remover/eliminar archivos del árbol de trabajo y del index
git restore <fileName>
git checkout -- <fileName> // !!!PRECAUCIÓN!!! Nos ayuda a descartar los cambios al archivo en cuestión ---No utilizar hasta estar completamente seguros de ello---
git mv <currentFileName> <newFileName> // Renombra archivos, pero GIT considera que se elimina un archivo y se crea uno nuevo
git log --decorate --oneline
git log --oneline
git log --graph
git log --oneline --graph
git log -<number>
git log --oneline -<number>
git log --graph -<number>
git log --oneline --graph -<number>
git log --pretty=format:"%h - %an, %ar : %s"
git log --after="YYYY-MM-DD HH:MM:SS"
git log --since="YYYY-MM-DD HH:MM:SS"
git log --before="YYYY-MM-DD HH:MM:SS"
git log --until="YYYY-MM-DD HH:MM:SS"
git log --after="YYYY-MM-DD HH:MM:SS" --before="YYYY-MM-DD HH:MM:SS"
git log --since="YYYY-MM-DD HH:MM:SS" --until="YYYY-MM-DD HH:MM:SS"
```

## No dar seguimiento a archivos/carpetas
*.gitignore*  
El archivo de configuración de GIT donde estableceremos los patrones de los nombres de  archivos y/o carpetas que no deseamos contemplar dentro de nuestro flujo de seguimiento con GIT de nuestro proyecto.  
Estructura base de un archivo **.gitignore**:  
```
app.js
*.css
node_modules
```