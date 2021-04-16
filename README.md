## :green_square: BÁSICO
### :green_circle: Primeros pasos con Git
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



## :blue_square: INTERMEDIO
### :large_blue_circle: Iniciando proyecto
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
### :large_blue_circle: Los 3 estados de Git
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
### :large_blue_circle: Restaura o deshace cambios realizados
#### git checkout 
##### Restaura
~~~
git checkout (Deshace cambios)
git checkout NombreArchivo (Deshace archivo con el nombre)
git checkout numeroCommit (Deshace archivo con el numero de commit)
git checkout --. (Deshace todos los archivos eliminados)
git checkout -f (restaura todos los cambios) 
git checkout master (restaura a ultimo commit)
~~~


#### git rm
~~~
git rm --cached NombreArchivo (Elimina archivos del árbol de trabajo y del índice) 
~~~


## :red_square: AVANZADO
### :red_circle: Personalizar Git
~~~
~~~
### :red_circle: Alias
~~~
git config --global alias.ATAJO "COMANDO"
git config --global -e (registro editable)
git config --global -l (lista de alias)
~~~
### :red_circle: Agregar archivos
![](https://i.ibb.co/HCm5grR/git-add.png)
### :red_circle: Crea Rama
~~~
git branch NombreRama (crea rama)
git checkout -b  (crea rama y se traslada)
~~~
### :red_circle: Cambiar de Rama
~~~
git switch NombreRama (Cambia de rama)
git checkout NombreRama (Cambia de rama)
git checkout master (Cambia a rama master)
~~~