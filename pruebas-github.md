# Pruebas con Github

## ¿Qué es este documento?

A través de este documento de mi repositorio de GitHub voy a explicar paso a paso cómo crear una cuenta en [GitHub](https://github.com) y cómo crear un repositorio.

<!--
En este punto he tratado de subir los cambios a GitHub, para ver si se muestran correctamente.
     --->

## ¿Qué es GitHub?

Es una plataforma de desarrollo colaborativo para alojar proyectos utilizando el sistema de control de versiones Git.

![Logo GitHub|100](https://global-uploads.webflow.com/5f5a53e153805db840dae2db/6073fbf151fa4565d48572dc_GitHub_aprender-programaci%25C3%25B3n.jpeg "Logo de GitHub")

## ¿Cómo creo un perfil en GitHub?

Para crear un perfil en GitHub hay que seguir los siguientes pasos:
1. Acceder a la [página principal de GitHub](https://www.github.com)

2. En la esquina superior derecha, pinchamos en **Sign Up**

3. Rellenar los siguientes campos:
	- **Nombre de usuario**: Elegir un nombre de usuario que esté disponible
	- **Contraseña**: Crear una contraseña que contenga números, letras (mayúsculas y minúsculas) y caracteres especiales
	- **Verificar la cuenta**: En la parte inferior de la página aparece un recuadro donde nos pide que verifiquemos la cuenta. Pinchamos y nos aparecerá una pregunta de seguridad para garantizar que no somos un robot. Resolvemos la pregunta y, si lo hemos hecho correctamente, aparecerá un símbolo que indica que nuestra cuenta ha sido verificada
	- **Crear cuenta**: Pinchamos sobre el botón **crear cuenta**

4. Ya estamos dentro de GitHub y nos plantean una serie de preguntas sobre sobre nuestra experiencia en programación y para qué vamos a usar GitHub. Podemos responder las preguntas o dejarlas sin responder.

5. Ya hemos creado un perfil. Si accedemos a la página "https://github.com/<tu nombre de usuario>", podremos personalizar nuestro perfil.

## ¿Cómo subo cambios de un documento a GitHub?

Para **subir al repositorio de GitHub** los cambios hechos en el ordenador hay que seguir los pasos siguientes:
1. Guardar los cambios en el documento:
	- En nano, pulsar **Control+X** para cerrar el documento
	- Cuando nano nos pregunte si queremos guardar los cambios, pulsamos **Control+Y** y **Intro**
	- Saldremos de nano y los cambios ya estarán gaurdados

2. Usar el comando **git status** para ver los cambios que hemos hecho en el ordenador y no se han actualizado en GitHub. Si hemos guardado los cambios correctamente, nos tendria que salir un mensaje como este:
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   pruebas-github.md

3. Generar un token en GitHub
	- Accedemos a la [página de creación de tokens](https://github.com/settings/tokens)
	- En el menú desplegable de la parte superior, pinchamos en *Generate token* y después seleccionamos **Generate new token (classic)**
	- Rellenar los siguientes campos:
		- **Note**: rellenar con un nombre descriptivo para nuestro token
		- **Expiration**: Seleccionar el tiempo de caducidad del token. Podemos dejar los 30 días que GitHub nos propone por defecto.
		- **Select scoptes**: Seleccionamos solo el campo *repo*
		- Pinchar en **Update token**
	- Una vez creado el token, lo copiamos (string largo de números y letras)

4. Volvemos al terminal y usamos el comando *git add <nombre del documento>*

5. Usamos el comando **git commit -m "<mensaje>"**. Dejamos un mensaje que describa los cambios que hemos hecho.

6. Usamos el comando **git push**. Nos aparecerá el siguiente mensaje:
	- Username for 'https://github.com': (Lo rellenamos con el nombre de usuario de GitHub y pulsamos la tecla Intro. No se verá en pantalla lo que estamos escribiendo.)

A continuación aparecerá el siguiente mensaje:
	- Password for 'https://spontsanchez@github.com': (Pegamos el token que hemos copiado anteriorente y pulsamos la tecla Intro. Tampoco se verá en pantalla lo que hemos pegado)

7. Cuando hayamos seguido estos pasos, vamos a nuestro repositorio de GitHub y comprobamos que el archivo se ha actualizado correctamente.
