











#### 9. git log
![](https://i.ibb.co/q1GBvC8/log-de-commit.png)
![](https://i.ibb.co/sWtjDx8/2021-03-31-17-31-55-3-3-Ramas-locales-mp4-Reproductor-multimedia-VLC.png)

~~~
git log (Muestran los registros de commits)
git log --oneline (muestra numero y commit)
git log --oneline -n 5 (muestra vista 5 ultimos)
git log --oneline --all (muestra todas las ramas)
git log --oneline --all --graph --decorate (muestra gráfica)
~~~


#### 17. git merge 
___Une dos o más historias___ de desarrollo juntas.

~~~
git merge NombreDeRama (une ramas)
~~~

##### Merge forward

![](https://i.ibb.co/T1J2qg5/fast-forward.png)

##### Merge Automática
![](https://i.ibb.co/vQmpRQF/automatica.png)

##### Merge Manual
![](https://i.ibb.co/G3GYFVP/manual.png)


#### 11. git reset
___Restablece HEAD___ actual al estado especificado.

~~~
git reset NombreArchivo (excluye archivo)
git reset HEAD NombreArchivo (deshace cambios en el archivo)
git reset --soft NumeroCommit (deshace commit)
git reset --soft HEADˆ (deshace ultimo commit)
git reset --hard NumeroCommit (deshace el commit y borra lo ultimo)
~~~

#### 12. git reflog 
Mantiene un registro de todo lo que se hace. Te salva la vida.
~~~
git reflog (Mantiene un registro de todo)
~~~

#### 13. git restore
___Restaura___ archivos de árbol de trabajo.

~~~
git restore --staget NombreArchivo
~~~

#### 14. git diff
___Muestra los cambios entre confirmaciones___, confirmaciones y árbol de trabajo, etc.

~~~
git diff --stat NombreArchivo (muestra estadistica de cambios)
git diff --staged (verifica archivos en staged)
~~~



#### 17. git tag
Crea, enumera, elimina o verifica un objeto de etiqueta firmado con GPG

~~~
git tag NombreTag (crea tag)
git tag -a VersionTag #commit -m "NombreTag" (crea tag desde commit) 
git tag (ver tags) 
git tag -d NombreTag (eliminar tag)
~~~

## Ignorar archivos
Crear archivo ".gitignore" dentro colocar la rutas de los archivos a ignorar y se puedo comentar con "# comentario".

~~~
carpeta/ignorar.txt (ruta) 
~~~