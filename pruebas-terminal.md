# Pruebas terminal

## Cygwin

Para empezar a usar **la terminal** hay que instalar **Cygwin** u otra interfície de línea de comandos. En nuestro caso, hemos instalado Cygwin.

### ¿Cómo se instala Cygwin?

- Descargar el ejecutable en la [web de Cygwin](https://www.cygwin.com/). El enlace se llama **setup-x86_64.exe** y se encuentra en el apartado **Installing Cygwin**.

- Durante la instalación tendremos que instalarnos los paquetes que vayamos a necesitar, en su versión más reciente. Para el máster de periodismo y visualización de datos, nos hemos instalado los siguientes paquetes y librerías:
	- Curl
	- Libcurl-devel
	- Libcurl4
	- Lynx
	- Git
	- Libgit2-devel
	- Ruby
	- Ca-certificates
	- Ca-certificates-letsencrypt
	- Wget
	- Wget2
	- Gcc-core
	- Libgcc1

## Comandos terminal

Algunos de los comandos básicos de la terminal son:
 - `cd` -> Cambiar directorio
 - `ls` -> Listar lo que hay dentro de un directorio
 - `'ls *.txt` -> Listar todos los documentos con formato .txt (se puede usar el mismo comando con cualquier otro formato)
 - `mkdir` -> Crear un directorio
 - `rm` -> Eliminar
 - `rmdir` -> Eliminar un directorio
 - `mv nombre_archivo directorio_destino` -> Mover archivo a otro directorio
 - `clear` -> Borrar la pantalla de la terminal
 - `cp archivo copiar_archivo` -> Copiar archivos y directorios (también se puede copiar en otro directorio)
 - `find` -> Buscar un archivo
 - `pwd` -> Nos imprime la ruta del directorio donde estamos
 - `whoami` -> Nos devuelve el nombre del usuario
 - `cat` -> Muestra el contenido de un archivo
 - `tail` -> Muestra las últimas filas del archivo
 - `wc` -> Cuentas las palabras, las líneas y los caracteres de un archivo
 - `--help` -> Aporta información sobre comandos y archivos de bash
 - `nano` -> Crear un archivo de nano o abrir un archivo de nano ya existente

## Cómo cambiar el tema de la terminal

Una opción es a través del archivo `.bashrc`. Entramos en el archivo con `nano` y cambiamos el contenido de la línia **THEME** con el tema que elijamos.

## ¿Qué es apt-cyg?

Apt-cyg es un gestor de paquetes para Cygwin, que nos permite instalar paquetes.

## ¿Qué es figlet?

Figlet es una aplicación informática que genera baners de texto con caracteres ASCII.
Podemos personalizar el texto de salida con los siguientes comandos:

 - `-f` para seleccionar una tipografía
 - `-d` para seleccionar el directorio de las tipografías
 - `-c` centra el texto de salida
 - `-l` alinea el texto a la izquierda.
 - `-r` alinea el texto a la derecha.
 - `-w` especifica un tamaño de salida.
 - `-k` habilita el kerning, creando cada letra de forma separada en vez de fundirse con las adyacentes.

## ¿Cómo se actualiza la variable PATH?

Para actualizar la variable `$PATH` hay que ejecutar la siguiente línea:

`export` `PATH=**la ruta que necesitemos incluir en la variable PATH**:$PATH`
