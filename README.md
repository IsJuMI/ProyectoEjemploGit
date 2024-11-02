# Práctica 1 : Introducción a Git
## Israel Julián Martínez

## Descripción
**Un sistema de control de versiones (vcs)**, es un mecanismo que permite almacenar, modificar y llevar un historial de código, en este curso estudiaremos Sistemas de Control de Versiones Distribuidas (DVCS). Git permite integrar los flujos de trabajo realizados por varios colaboradores a lo largo del tiempo en un repositorio determinado. por su parte GitHub(provedor de alojamiento) es un servicio de hospedaje basado en web de repositorios de Git. En está práctica realizamos la creación de un archivo HolaMundo.py agregamos el mensaje de primer commit "Se agregó el programa de Hola Mundo en Python", Despues creamos u archivo debug,log y el archivo .gitignore para ignorar los archivos.log y al realizar el segundo commit agregamos el mensaje "Se agregó el archivo ,gitignore", posteriormente checamos que el archivo debug.log fuera ignorado al usar el comando git status. Por último actualizamos HolaMundo.py y en el commit agregamos el mesaje "Se actualizó el mensaje de HolaMundo.py". Cabe destacar que en mi repositorio de git se encuentran los commit que realizé y contiene el historial de los commit . 
### Objetivo de la práctica
**El objetivo de la práctica es aprender a usar la herramienta GitHub, usando los comandos explicados en la sección de "Comandos utilizados", como referencia puedo decir que me apoye con el video realizados por el Dr. Ismael Robles quien explica detalladamente los pasos a seguir para poder usar Git. La práctica tiene tambien el objetivo de enteder como es un sistema distribuido y las ventajas que te puede dar. En lo personal es la primera vez que uso esta herramienta pero me parecio una fantastica herramienta ya que para los programadores que en lo general trabajan un proyecto en equipo les facilita la creación de un sistema puesto que pueden subir a un mismo repositorio el avance de cada integrante.**

## Instrucciones de uso
Un sistema distribuido se basa en tener un servidor de computadora que funge como repositorio remoto y al cual estan conectadas computadoras, de esta forma se asegura que tengamos un respaldo de información y podamos acceder a ella.
Para usar Git debemos se requiere un cliente Git y un servidor de Git, usualmente se usa un proveedor de repositorios Git.
Para ejecutar el programa HolaMundo.py podemos darle doble clic y descargar el archivo individualmente, tambien lo podemos ejecutar en el editor de tu preferencia. Por otra parte, podemos hacer una copia de uestro repositorio remoto  a nuestro equipo usando  el comando **git clone URL** explicado a más detalle en la seccioón de comandos utilizados.
* Para esta práctica usamos Markdown es un lenguaje de marcado que facilita la aplicación de formato a un texto empleando una serie de caracteres de una forma especial,fue pensado para elaborar textos cuyo destino iba a ser la web con más rapidez y sencillez que si estuviésemos empleando directamente HTML. Si bien ese suele ser el mejor uso que podemos darle, también podemos emplearlo para cualquier tipo de texto, independientemente de cual vaya a ser su destino.*

## Comandos utilizados
#### Inicialización del cliente Git
Para inicializar el cliente Git usamos los siguientes comandos:
+ **git config --global user.name "Israel Julián Martínez"** *Poner nuestro nombre dentro de las comillas*
+ **git config --global user.email "cidseul@gmail.com"** *Se debe usar el correo de registro en github*

### Inicializar un repositorio local y remoto
#### Inizializar el repositorio local
+ **git init** *Se usa para inicializar el repositorio, se debe ejecutar desde la raiz de nuestra carpeta raiz de nuestro proyecto*
+ **git remote add Origin https://github.com/IsJuMI/ProyectoEjemploGit.git** *Se debe usar usualmente en lugar de Alias=Origin y se debe de poner la URL de nuestro repositorio, se enlaza el repositorio local y el remoto*
+ **Touch .gitignore** *Se crea un archivo que permite ignorar ciertos archivos que no queremos que esten bajo el control de git*
#### Enviar cambios al repositorio remoto
+ **git add -A** *Usamos este comando para enviar todos los archivos del directorio de trabajo(working directory) al al área de preparación(staging area)*
+ **git add HolaMundo.py** *Usamos este comando para enviar solamente un archivo del directorio de trabajo(working directory) al al área de preparación(staging area)*
+ **git commit -m** *Usamos este comando para pasar del área de preparación(staging area) al repositorio local(local repo), es una operación de confirmación*
+ **git commit -m "Se actulizó el mensaje en HolaMundo.py"** *Usamos este comando para pasar del área de preparación(staging area) al repositorio local(local repo), use el mensaje de actualización para que en mi repositorio tuviera una etiqueta de los commit que hice*
+ **git status** *Con este comando podemos ver el estatus de los archivos, si estan el el directorio de trabajo o en el repositorio local.*
+ **git push origin master** *con el comando enviamos todos los commit del repositorio local(local repo) al repositorio remoto(remote repo).
+ Después de realizar la práctica comprobe en github que habia realizado 3 commits en total, el primer commit de "Hola mundo", el segundo para "Se agregó el archivo .gitignore" y el tercero para "Se actulizó el mensaje en HolaMundo.py".
+ **git clone URL** *Con el comando se obtiene una copia desde el repositorio remoto, el URL debe ser de nuestro repositorio.* *Cabe mencionar que podemos agregar un nuevo nombre agregandolo después del URL, de otro modo el no,bre de la copia será el mismo que tiene en el repositorio local* La copia se almacenara en nuestra repositorio local.*
+ **git pull origin master** *Con este comando se actualiza el repositorio local con cambios del repositorio remoto*

## Notas sobre el archivo .gitignore
+ **Touch .gitignore** *Se crea un archivo que permite ignorar ciertos archivos que no queremos que esten bajo el control de git, en este archivo podemos poner a todos los tipos de archivos que queremos ignorar*
+ /debug.log *Ignara el archivo "debug.log*
+ debug.log *Ignora cualquier archivo con el nombre debug.log*
+ *.log *Ignora cualquier archivo de extención .log*
+ **/logs *Ignora todas las carpetas logs*
+ **Un archivo local .gitignore generalmente se coloca en el directorio raíz de un proyecto. Tambien se puede crear un archivo global .gitignore, y cualquier entrada en ese archivo se ignorará en todos tus repositorios de Git.**

### Referencias
**[1] ,Genbeta, "Qué es Markdown", https://www.genbeta.com**
**[2], Dr. Ismael Robles, "Introcucción a Git", https://www.youtube.com**


