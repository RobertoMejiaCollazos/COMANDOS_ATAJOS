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