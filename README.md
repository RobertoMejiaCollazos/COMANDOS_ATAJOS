## :orange_square: BÁSICO
### :orange_circle: Primeros pasos con Git
#### git version
~~~
git version (ver si esta instalado)
~~~
#### git help 
~~~
git help (Muestra comandos existentes)
git help NombreComando (Muestra descripción del comando)
~~~
#### git config 
Obtiene y configura el repositorio o las opciones globales.
~~~
git config global --user.name "Nombre del autor"
git config global --user.email "Correo del autor"
~~~
~~~
git config --list (muestra las configuraciones de git)
~~~



## :yellow_square: INTERMEDIO
### :yellow_circle: Iniciando proyecto
#### git init
~~~
git init (Crea un repositorio local (.git) o reinicia uno)
~~~
#### git status
~~~
git status (Muestra el estado del árbol de trabajo)
git status -s ("s" de silent o silencioso)
git status -s -b ("silent" y "branch")
git status -sb (igual "-s -b")
~~~
### :yellow_circle: Los 3 estados de Git
1. Espacio de trabajo
2. Area de preparación
3. Repositorio (carpeta .git)

![](https://i.ibb.co/16LXjLM/3estados.png)

#### git add 
~~~
git add (Agrega el contenido del archivo al indice)
git add NombreArchivo (Agrega archivo)
git add . (Manda todo a "staging area")
git add -A (Manda todo a "staging area")
git add --all (Manda todo a "staging area")
~~~
#### git commit
~~~ 
git commit (Registra los cambios en el repositorio)
git commit -m "NombreCommit" (registra commit)
git commit -am "NombreCommit" (registra solo modificados)
git commit --amend (Registro de commit)
git commit --amend -m "NombreCommit" (Renombrar)
~~~
#### git log
![](https://i.ibb.co/q1GBvC8/log-de-commit.png)
![](https://i.ibb.co/sWtjDx8/2021-03-31-17-31-55-3-3-Ramas-locales-mp4-Reproductor-multimedia-VLC.png)
~~~
git log (Muestran los registros de commits)
git log --oneline (muestra numero y commit)
git log --oneline -n 5 (muestra vista 5 ultimos)
git log --oneline --all (muestra todas las ramas)
git log --oneline --all --graph --decorate (muestra gráfica)
~~~
#### git reset
~~~
git reset (Restablece HEAD actual al estado especificado)
git reset NombreArchivo (excluye archivo)
git reset HEAD NombreArchivo (deshace cambios en el archivo)
git reset --soft NumeroCommit (deshace commit)
git reset --soft HEADˆ (deshace ultimo commit)
git reset --hard NumeroCommit (deshace el commit y borra lo ultimo)
~~~
### :yellow_circle: Restaura o deshace cambios realizados
#### git checkout 
~~~
git checkout (Deshace cambios)
git checkout NombreArchivo (Deshace cambios del archivo)
git checkout carpeta/Archivo (Deshace cambios del archivo)
git checkout numeroCommit (Deshace cambios del commit)
git checkout --. (Deshace todos los archivos eliminados)
git checkout -f (restaura todos los cambios) 
git checkout master (restaura a ultimo commit)
~~~
#### git rm
~~~
git rm --cached NombreArchivo (Elimina archivos del árbol de trabajo y del índice) 
~~~
### :yellow_circle: Trabajando con ramas
#### git branch
~~~
git branch (ver todas las ramas)
git branch NuevaRama (Crea rama)
git branch -D NombreRama (elimina rama)
git branch -d NombreRama (elimina rama)
~~~
#### git merge 
~~~
git merge (Une dos o más historias de desarrollo juntas)
git merge NombreRama (Une la rama master con otra rama)
~~~
###### Merge forward
![](https://i.ibb.co/T1J2qg5/fast-forward.png)
###### Merge Automática
![](https://i.ibb.co/vQmpRQF/automatica.png)
###### Merge Manual
![](https://i.ibb.co/G3GYFVP/manual.png)


## :blue_square: AVANZADO
### :large_blue_circle: Personalizar Git
~~~
~~~
### :large_blue_circle: Alias
~~~
git config --global alias.ATAJO "COMANDO"
git config --global -e (registro editable)
git config --global -l (lista de alias)
~~~
### :large_blue_circle: Agregar archivos
![](https://i.ibb.co/HCm5grR/git-add.png)
### :large_blue_circle: Crea Rama
~~~
git branch NombreRama (crea rama)
git checkout -b  (crea rama y se traslada)
~~~
### :large_blue_circle: Cambiar de Rama
~~~
git switch NombreRama (Cambia de rama)
git checkout NombreRama (Cambia de rama)
git checkout master (Cambia a rama master)
~~~