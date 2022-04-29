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
git diff --staged
git reset HEAD <fileName>
git commit --amend
git commit -a -m
git rm <fileName>
git restore <fileName>
git checkout -- <fileName>
git mv <actualFileName> <newFileName>
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