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
git add <filename>
git add .
git add -A
git status
git commit m- "Your descriptive commit description goes here"
git log
git diff
git diff --staged
git reset HEAD <fileName>
git commit --amend
```

## No dar sequimiento a archivos/carpetas
*.gitignore*  
El archivo de configuración de GIT donde estableceremos los patrones de los nombres de  archivos y/o carpetas que no deseamos contemplar dentro de nuestro flujo de seguimiento con GIT de nuestro proyecto.  
Estructura base de un archivo **.gitignore**:  
```
app.js
*.css
node_modules
```