# Práctica 1 : Introducción a Git
## Israel Julián Martínez

## Descripción
**Un sistema de control de versiones (vcs)**, es un mecanismo que permite almacenar, modificar y llevar un historial de código, en este curso estudiaremos Sistemas de Control de Versiones Distribuidas (DVCS). Git permite integrar los flujos de trabajo realizados por varios colaboradores a lo largo del tiempo en un repositorio determinado. por su parte GitHub(provedor de alojamiento) es un servicio de hospedaje basado en web de repositorios de Git.
### Objetivo de la práctica


## Instruccines de uso
Para ejecutar el programa HolaMundo.py podemos darle doble clic y descargar el archivo, posteriormente lo podemos ejecutar en el editor de tu preferencia.

## Comandos utilizados
### Inicialización del cliente Git
Para inicializar el cliente Git usamos los siguientes comandos:
+ **git config --global user.name "Israel Julián Martínez"** *Poner nuestro nombre dentro de las comillas*
+ **git config --global user.email "cidseul@gmail.com"** *Se debe usar el correo de registro en github*

### Inicializar un repositorio local y remoto
#### Inizializar el repositorio local
+ **git init** *Se usa para inicializar el repositorio, se debe ejecutar desde la raiz de nuestra carpeta raiz de nuestro proyecto*
+ **git remote add Origin https://github.com/IsJuMI/ProyectoEjemploGit.git** *Se debe usar usualmente en lugar de Alias=Origin y se debe de poner la URL de nuestro repositorio, se enlaza el repositorio local y el remoto*
+ **Touch .gitignore** *Se crea un archivo que permite ignorar ciertos archivos que no queremos que esten bajo el control de git*
#### Enviar cambios al repositorio remoto
+ **git add -A** *Poner nuestro nombre dentro de las comillas*
+ **git commit -m** *Se debe usar el correo de registro en github*
+ **git push** 
# Notas sobre el archivo .gitignore
+ /debug.log *Ignara el archivo "debug.log"
+ debug.log *Ignora cualquier archivo con el nombre debug.log*
+ *.log *Ignora cualquier archivo de extención .log*
+ **/logs *Ignora todas las carpetas logs*
