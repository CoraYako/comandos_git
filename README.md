# Programación I Comandos Git y GitBash (UTN)

## Información
Alumno: Héctor Armando Cortez ([LinkedIn](https://www.linkedin.com/in/hector-cortez-cy/))
<br>
Institución: [UTN Facultad Regional San Rafael](https://www.frsr.utn.edu.ar/)
<br>
Asignatura: Programación I GitBash
<br>
Profesor: Profesor Ariel Betancud ([GitHub](https://github.com/ArielBetancud22))
<br>
Grupo: DinamicDevs
<br>
Cohorte: 2024

A continuación se detalla lo visto en cada clase de Git y comandos de Terminal en la Tecnicatura Universitaria en Programación de la [UTN Facultad Regional San Rafael](https://www.frsr.utn.edu.ar/). Utilice el índice debajo para navegar entre las clases impartidas.

* [Clase Miércoles 27 de Marzo del 2024](#clase-miércoles-27-de-marzo-del-2024)
    * [Clase Anterior](#lo-que-vimos-en-la-clase-anterior)
    * [Creación de Carpetas](#ahora-comenzamos-con-la-creación-de-carpetas)
* [Clase Miércoles 3 de Abril del 2024](#clase-miércoles-3-de-abril-del-2024)
    * [Crear Repositorio Git](#crea-un-repositorio-de-git-y-haz-tui-primer-commit)
* [Clase Miércoles 10 de Abril del 2024](#clase-miércoles-10-de-abril-del-2024)
    * [Analizar Cambios en los Archivos de tu Proyecto Git](#analizar-cambios-en-los-archivos-del-proyecto-git)
## CLASE MIÉRCOLES 27 DE MARZO DEL 2024
### Lo que vimos en la clase anterior:
> Abrimos la terminal de **Git Bash** en **Windows** o la terminal de **Ubuntu**, tambien la terminal de **Mac**, y comenzamos con los siguientes comandos y creación de directorios:
> - ``pwd`` Vemos la ruta de la carpeta en la que estamos.
> - ``cd`` Es para navegar a una carpeta: change directory -> cambiar de directorio.
> - ``cd /`` Nos llava al home, en la raíz del disco.
> - ``cd ~`` La virgulilla significa que estamos en el lugar de los documentos o del usuario.
> - ``ls`` Esto es listar los archivos, nos muestra todos los archivos en la raíz.
> - ``ls -al`` El espacio ``-al`` significa que es un argumento especial para ver _archivos ocultos_.
> - Usar la flecha hacía arriba nos muestra el último comando utilizado.
> - ``ls -l`` Muestra casi todos los archivos sin los que están ocultos.
> - ``ls -a`` Muestra el grupo de archivos pero no en una lista.
> - ``clear`` Limpia la consola o Ctrl + L.
> - ``cd ..`` Nos devuelve a la carpeta anterior.
> - ``cd U + Tab`` Esto se usa para un autocompletado o para buscar una referencia.
> - ``cd /D`` Cambiamos de disco en window.
> - ``df -h`` Muestra todos los directorios en __Ubuntu__.
> - ``cd /mnt/d`` Cambia de directorio usando __WSL Ubuntu en Windows__.

### Ahora Comenzamos con la Creación de Carpetas
Abrimos la terminal de Git Bash y tecleamos los siguientes comandos.
<br>
Importante seguir los pasos uno a uno.

1. ``cd ..`` nos llevará a nustra carpeta de usuario

2. ``cd ..`` nos lleva al disco principal de nuestra PC
3. ``cd /mnt/c`` para cambiar el directorio
4. ``cd ~`` para ir a la raíz
5. ``mkdir Tecnicatura`` para crear la carpeta Tecnicatura
6. ``cd tecnicatura`` para ingresar a la carpeta creada en el paso anterior
7. ``mkdir Python``
8. ``mkdir Java``
9. ``mkdir JavaScript``

> [!NOTA]
> Recordar que en window las mayúsculas no tienen relevancia, pero si en Linux

Revisar y ejecutar cada comando, hacerlo como practica.

## CLASE MIÉRCOLES 3 DE ABRIL DEL 2024
Abrir git bash en **Windows** o la terminal de __Linux__ o de __Mac__: al abrir Git Bash hacerlo como administrador.

Crea un archivo con su extención.
- ``touch nombre-archivo.txt``

Una vez creado, abrirlo y escribir unas líneas dentro.Ctrl + S para guardar lo que escribimos en el archivo.

- ``./`` Significa la carpeta actual
- ``../`` Significa la carpeta anterior
- ``cat nombre-archivo.txt`` Vemos el contenido del archivo
- ``history`` Veremos la historia completa de los comandos que hemos utilizado
- ``!72 + enter`` Veremos el comando que utilizamos en ese número
- ``rm nombre-archivo.txt`` Borra el archivo seleccionado.

> [!ADVERTENCIA]
> La acción ``rm nombre-archivo.txt`` no se puede deshacer.

- ``rm --help`` Muestra como funciona el comando

### Crea un repositorio de Git y haz tui Primer Commit
Realizada la ejecución de cada comando en el orden especificado.
1. Ingresamos a la carpeta creada en la [primer clase](#ahora-comenzamos-con-la-creación-de-carpetas) con el siguiente comando: ``cd tecnicatura``

2. Creamos la carpeta class-git con el siguiente comando: ``mkdir class-git``
3. Entramos en la carpeta que necesitamos trabajar: ``cd class-git``
4. Creamos un repositorio en la carpeta central: ``git init``. Se crea el archivo .git (este archivo está oculto por defecto).
5. Abrimos VSC: ``code .`` el punto hace que se abra el archivo en el que estamos situados.
6. Ya en Visual Studio Code, creamos un archivo nuevo con Ctrl + N y escribimos en él.
7. Guardamos el archivo con Ctrl + S poniendo el nombre: _historia.txt_
8. Vemos el estado del proyecto en tiempo real con el comando ``git status`` y vemos que esta en el área de trabajo.
9. Enviamos el archivo al área de preparación con ``git add historia.txt``
10. Para ver el estado de cambios escribimos ``git status``
11. Quitamos el archivo del área de preparación con ``git rm --cached historia.txt``, ``cached`` significa que esta en memoria RAM.
12. Con ``git config`` tedremos la lista de como funciona la configuración de Git.
13. Escribimos ``git config --list`` para ver las configuraciones por defecto, faltan cosas importantes. Para salir de la vista precionar la tecla Q.
14. Para ver dónde están guardadas las configuraciones guardadas, escribimos el diguiente comando: ``git config --list --show-origin``
15. Para configurar un nombre se usuario en Git, escribir lo siguiente en la terminal: ``git config --global user.name "Tu Nombre Completo". Dentro de las comillas dobles colocar tu nombre completo.``
16. De la misma forma que antes, vamos a establecer un valor para el correo en Git con el siguiente comando: ``git config --global user.email "tu_correo@correo.com"``.  Dentro de las comillas dobles colocar tu correo personal.

> [!Importante]
> Colocar un correo válido y personal, ya que utilizaremos el mismo para crear una cuenta en [GitHub](https://github.com/).

17. Listamos nuevamente las configuraciones de Git con ``git config --list`` y veremos que ya están todos nuestros datos completos.

18. Ingresamos todos los archivos al área de preparación (RAM) con el siguiente comando: ``git add .``
19. Escribimos lo siguiente en la terminal: ``git commit -m "Mensaje importante del commit"``. El mensaje dentro de las comillas sirve para identificar qué cambios o modificaciones se realizaron en el o los archivos. Por esta razón debemos colocar un mensaje descriptivo para cada commit que realicemos.
20. Volvemos a abrir nuestro Visual Studio Code ``code .`` y hacemos cambios en el archivo, luego guardamos.
21. Revisamos nuestra área de trabajo con ``git status`` y vemosz que hay cambios para _commitear_.
22. Los agregamos al área de preparación con ``git add .``
23. Creamos otro commit con ``git commit -m "Mensaje importante del commit"``
24. Por último vemos todo el historial de este archivo con ``git log historia.txt``. El número largo es el hash o _identificador_ del commit.

Revisar y ejecutar cada comando, hacerlo como practica.

## CLASE MIÉRCOLES 10 DE ABRIL DEL 2024
### Analizar Cambios en los Archivos del Proyecto Git

Ingresamos de la siguiente manera:
<br>
Abrir git bash en __Windows__ o la terminal de __Linux__ o de __Mac__: al abrir Git Bash hacerlo como _administrador_, en terminal también o usar ``sudo`` para permisos especiales.

- ``cd tecnicatura`` Ingresamos al direcotorio donde están nuestras carpetas de trabajo

- ``ls`` Vemos los archivos y directorios que ya tenemos

- ``cd git`` No hay nada

- ``cd ..`` Salimos

- ``rm historia.txt`` Eliminamos el archivo que habíamos hecho, esto en git bash (Windows) esto es para practica

- ``rm Git`` Al intentar el comando anterior recibimos el siguiente mensaje:
> rm: cannot remove 'Git': Is a directory

- ``rm --recursive -R Git`` Al intentar el comando anterior recibimos el siguiente mensaje:
> By default, rm does not remove directories.  Use the --recursive (-r or -R) arguments option to remove each listed directory, too, along with all of its contents 

- ``rm --help`` Nos muestra lo que les puse arriba como documentación en Inglés.

- ``mkdir class-git`` Creamos la carpeta o directorio para trabajar en Git local por ahora.

- ``cd class-git`` Entramos para crear el __README.md__ para este sector.

- ``touch README.md`` Vamos a crear un archivo nuevo, ``md`` significa _markdown_ y se pueden trabajar con editores de texto. Este es un lenguaje que transforma el texto a html.

- Enlace a la documentación en GitHub de [MARKDOWN](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

- Leemos la documentación para ir creando en __README.md__ como lo enseña GitHub.

- ``code .`` Para abrir VSC y editar el archivo.

- Empezamos a cargar lo visto en las clases anteriores (Comandos) en el README y pasamos a commitear.

- Realizamos los siguientes comandos en orden:
```
git status

git add .

git status

git commit -m "Cargamos el README dentro del directorio class-git"

git status
```
- ``git log`` Para ver los dos commits hechos: Si tienes commiteada alguna clase anterior veras mas commits dentro.

- ``cd ..`` Para salir de la carpeta actual (class-git)

- ``cd ..`` Para salir de la carpeta actual (Tecnicatura) y volver a la raíz

Revisar y ejecutar cada comando, hacerlo como practica
