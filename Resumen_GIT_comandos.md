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
-     git add . (Agrega todos los cambios)
#### 7. git commit
Registra los cambios en el repositorio. 
-     git commit -m "Nombre del commit" (Creando commit)
-     git commit -am "Nombre del commit" (Creando commit solo para archivos modificados)
-     git commit --amend (modifica el nombre del commit)
#### 8. git log
Muestran los registros de confirmación.

##### Ramas
![master](https://i.ibb.co/q1GBvC8/log-de-commit.png)
![Ramas](https://i.ibb.co/sWtjDx8/2021-03-31-17-31-55-3-3-Ramas-locales-mp4-Reproductor-multimedia-VLC.png)

-     git log --oneline (vista resumida)
-     git log --oneline -n 5 (vista personalizada)
-     git log --oneline --all (visualiza todas las ramas)
-     git log --oneline --all --graph
-     git log --oneline --all --graph --decorate (gráfica)
#### 9. git checkout 
Cambia de rama o restaura archivos de árbol de trabajo.
-     git checkout NombreArchivo (restaura archivo)
-     git checkout -f (todos los cambios se resetean)
-     git checkout -b NombreRama ("b" de branch o rama)
#### 10. git restore
-     git restore --staget nombre del archivo
#### 11. git diff
-     git diff --stat NombreArchivo (muestra estadistica de cambios)
#### 12. git switch
Cambia de rama al igual que "git checkout -b nombre de rama".
#### 13. git branch
Enumera, crea o elimina ramas..
#### 14. git merge 
Une dos o más historias de desarrollo juntas.
