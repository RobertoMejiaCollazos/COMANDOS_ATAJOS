# GIT
- - -
Git es un software de control de versiones diseñado por ___Linus Torvalds___, pensando en la eficiencia, la confiabilidad y compatibilidad del mantenimiento de versiones de aplicaciones cuando estas tienen un gran número de archivos de [código fuente](https://es.wikipedia.org/wiki/C%C3%B3digo_fuente). Su propósito es llevar registro de los cambios en archivos de computadora incluyendo coordinar el trabajo que varias personas realizan sobre archivos compartidos en un repositorio de código.
## Primeros comandos
#### 1. git version

#### 2. git help 
-     git help (Muestra lista de comandos existentes)
-     git help "nombre de comando sin comillas"
#### 3. git config 
Obtiene y configura el repositorio o las opciones globales.
-     git config --global user.name "usuario"
-     git config --global user.email "correo"
-     git config --global -e

## Iniciando un proyecto
Los 3 estados de Git
#### 4. git init
Crea un repositorio de Git o rehinicia uno.
#### 5. git status
Muestra el estado del árbol de trabajo.
![Los estados de git](https://i.ibb.co/HhBsyqf/los-estados-de-git.png)
#### 6. git add 
Agrega el contenido del archivo al indice.
-     git add .
#### 7. git commit
Registra los cambios en el repositorio. 
-     git commit -m "Nombre del commit"
-     git commit -am "Solo para archivos modificados"
-     git commit --amend (modifica el nombre del commit)
#### 8. git log
Muestran los registros de confirmación. 
![master](https://i.ibb.co/q1GBvC8/log-de-commit.png)
#### 9. git checkout 
Cambia de rama o restaura archivos de árbol de trabajo.
-     git checkout nombre del archivo (Cambia de rama o restaura archivos del árbol de trabajo)
-     git checkout -f (todos los cambios se resetean)
10. git restore
-     git restore --staget "nombre del archivo sin comillas"
11. git diff
-     git diff --stat ()
