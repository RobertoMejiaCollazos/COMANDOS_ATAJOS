#### git reset
~~~
git reset (Restablece HEAD actual al estado especificado)
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