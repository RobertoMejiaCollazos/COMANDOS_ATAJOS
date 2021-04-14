# GitHub
GitHub es una forja (plataforma de desarrollo colaborativo) para alojar proyectos utilizando el sistema de control de versiones Git. Se utiliza principalmente para la creación de código fuente de programas de ordenador. El software que opera GitHub fue escrito en Ruby on Rails. Desde enero de 2010, GitHub opera bajo el nombre de GitHub, Inc. Anteriormente era conocida como Logical Awesome LLC. El código de los proyectos alojados en GitHub se almacena típicamente de forma pública.

El 4 de junio de 2018 Microsoft compró GitHub por la cantidad de 7500 millones de dólares1​2​, al inicio el cambio de propietario generó preocupaciones y la salida de algunos proyectos de este repositorio3​, sin embargo no fueron representativos. GitHub continua siendo la plataforma más importante de colaboración para proyectos Open Source.

## Repositorio Remoto

![](https://i.ibb.co/Lx99GGG/push.png )

#### 1. git clone
___Clona un repositorio___ en un nuevo directorio.

~~~
git clone URL (descarga copia)
~~~

#### 2. remote
Administra un conjunto de repositorios rastreados 

~~~
git remote -v (origin y rama)
~~~
#### 3. git push
___Actualiza___ las referencias remotas junto con los objetos asociados.

~~~
git push origin master (nombre de rama)
git push --delete origin rama (elimina rama de github)
~~~

#### 4. git fetch  
Descarga objetos y referencias de otro repositorio.
~~~
git fetch 
~~~

#### 5. git pull
___Obtenga e integre___ con otro repositorio o una sucursal ___local___

~~~
git pull origin master (nombre de rama) 
~~~