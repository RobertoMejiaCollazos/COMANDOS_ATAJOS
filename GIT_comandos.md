# GIT
Git es un software de control de versiones diseñado por ___Linus Torvalds___, pensando en la eficiencia, la confiabilidad y compatibilidad del mantenimiento de versiones de aplicaciones cuando estas tienen un gran número de archivos de [código fuente](https://es.wikipedia.org/wiki/C%C3%B3digo_fuente). Su propósito es llevar registro de los cambios en archivos de computadora incluyendo coordinar el trabajo que varias personas realizan sobre archivos compartidos en un repositorio de código.

## Primeros comandos
#### 1. git version

#### 2. git help 
~~~
git help (Muestra comandos existentes)
git help NombreComando
~~~
#### 3. git config 
Obtiene y ___configura___ el repositorio o las opciones globales.

##### Configura ___usuario y correo___
~~~
git config --global user.name "usuario"
git config --global user.email "correo"
~~~

##### Configura ___alias___

~~~
git config --global alias.ATAJO "COMANDO"
git config --global -e (registro editable)
git config --global -l (lista de alias)
~~~

## Iniciando un proyecto

Los 3 estados de Git
![Los estados de git](https://i.ibb.co/HhBsyqf/los-estados-de-git.png)

#### 4. git init
Crea un repositorio de Git o reinicia uno (se crea la rama master). 
![Git init](https://i.ibb.co/mvG0rbB/git-init.png)

#### 5. git status
Muestra el ___estado___ del árbol de trabajo.

~~~
git status -s ("s" de silent o silencioso)
git status -s -b ("silent" y "branch")
git status -sb (igual "-s -b")
~~~

#### 6. git add 
___Agrega___ el contenido del archivo al indice.

~~~
git add . (Agrega todos los cambios)
git add --all (Agrega todos los cambios)
git add -A (Agrega todos los cambios)
~~~

![Comandos git add](https://i.ibb.co/HCm5grR/git-add.png)

#### 7. git commit
___Registra___ los cambios en el repositorio.

~~~ 
git commit -m "NombreCommit" (registra commit)
git commit -am "NombreCommit" (registra solo modificados)
git commit --amend (Registro de commit)
git commit --amend -m "NombreCommit" (Renombrar)
~~~

#### 8. git log
Muestran los ___registros de confirmación___.

##### Ramas

![master](https://i.ibb.co/q1GBvC8/log-de-commit.png)
![Ramas](https://i.ibb.co/sWtjDx8/2021-03-31-17-31-55-3-3-Ramas-locales-mp4-Reproductor-multimedia-VLC.png)

~~~
git log --oneline (muestra numero y commit)
git log --oneline -n 5 (muestra vista 5 ultimos)
git log --oneline --all (muestra todas las ramas)
git log --oneline --all --graph --decorate (muestra gráfica)
~~~

#### 9. git checkout 
___Cambia de rama o restaura___ archivos de árbol de trabajo.

##### Crea Rama
![rama2](https://i.ibb.co/bRFpsdq/rama.png)

~~~
git checkout -b CreaNombreRama ("b" de branch o rama)
~~~
##### Restaura
~~~
git checkout --. (restaura todos los archivos eliminados)
git checkout NombreArchivo (restaura archivo con el nombre)
git checkout numeroCommit (restaura archivo con el numero de commit)
git checkout -f (restaura todos los cambios) 
git checkout master (restaura a ultimo commit)
~~~

#### 10. git reset
___Restablece HEAD___ actual al estado especificado.

~~~
git reset NombreArchivo (excluye archivo)
git reset HEAD NombreArchivo (deshace cambios en el archivo)
git reset --soft NumeroCommit (deshace commit)
git reset --soft HEADˆ (deshace ultimo commit)
git reset --hard NumeroCommit (deshace el commit y borra lo ultimo)
~~~

#### 11. git reflog 
Mantiene un registro de todo lo que se hace. Te salva la vida.
~~~
git reflog (Mantiene un registro de todo)
~~~

#### 11. git restore
___Restaura___ archivos de árbol de trabajo.

~~~
git restore --staget NombreArchivo
~~~

#### 12. git diff
___Muestra los cambios entre confirmaciones___, confirmaciones y árbol de trabajo, etc.

~~~
git diff --stat NombreArchivo (muestra estadistica de cambios)
git diff --staged (verifica archivos en staged)
~~~

#### 13. git switch
___Cambia de rama___ al igual que "git checkout -b nombre de rama".

#### 14. git branch
Enumera, crea o elimina ramas.

~~~
git branch (ver todas las ramas)
git branch -D NombrRama (elimina la rama)
~~~

#### 15. git merge 
___Une dos o más historias___ de desarrollo juntas.

##### Merge forward

![](https://i.ibb.co/T1J2qg5/fast-forward.png)

##### Merge Automática
![](https://i.ibb.co/vQmpRQF/automatica.png)

##### Merge Manual
![](https://i.ibb.co/G3GYFVP/manual.png)

~~~
git merge NombreDeRama (une ramas)
~~~

#### 16. git clone
___Clona un repositorio___ en un nuevo directorio.

~~~
git clone URL (descarga copia)
~~~

#### 17. remote
Administra un conjunto de repositorios rastreados 

~~~
git remote -v (origin y rama)
~~~
#### 18. git push
___Actualiza___ las referencias remotas junto con los objetos asociados.

~~~
git push origin master (nombre de rama)
git push --delete origin rama (elimina rama de github)
~~~

#### 19. git fetch  
Descarga objetos y referencias de otro repositorio.
~~~
git fetch 
~~~

#### 20. git pull
___Obtenga e integre___ con otro repositorio o una sucursal ___local___

~~~
git pull origin master (nombre de rama) 
~~~

## Ignorar archivos
Crear archivo ".gitignore" dentro colocar la rutas de los archivos a ignorar y se puedo comentar con "# comentario".

~~~
carpeta/ignorar.txt (ruta) 
~~~