# Configuracion de Repositorio

## Configuracion Git Local - MacOS Big Sur
01. Descargar e instale git a través de la terminal de Mac con Homebrew con el comando `brew install git`.
02. Confirmo la instalación consultando la versión con el comando `git --version`.
03. Configuro el usuario y correo:
    ❯ git config --global user.name "Esteban Saxton"
    ❯ git config --global user.mail "e.saxton@go.ugr.es"
04. En la terminal crear clave ssh con el comando `ssh-keygen -t ed25519 -C "tucorreo@github.es"`.
05. Cambiar el NOMBRECLAVE ssh o dejar el que viene por defecto.
06. Ingresar una passphrase y luego lo repetir la misma.
07. Iniciar ssh-agent con el comando `eval "$(ssh-agent -s)"`
08. Crear el archivo de configuracion en el directorio .ssh con el comando `touch ~/.ssh/config`
09. Editar el archivo config agregando lo siguiente y remplazando el nombre de la llave por el que le dimos en el paso 5:
    Host *
        AddKeysToAgent yes
        UseKeychain yes
        IdentityFile ~/.ssh/NOMBRECLAVE
10. Agregar la clave privada SSH al ssh-agent con el comando `ssh-add -K ~/.ssh/NOMBRECLAVE`
11. Ingresar a la carpeta donde generó la clave ssh y abrir el archivo .pub con VS Code. 
12. Copiar el contenido en el portapapeles.

## Configuración GitHub
13. Ingresar a settings y seleccionar en el menú lateral SSH and GPG keys.
14. Clicar en el boton New SSH key.
15. Ingresar un nombre descriptivo del dispotivo que tiene esa SSH Key y luego pegar lo que guarde en el portapales (Configuración Git Local , paso 12).
16. Finalmente clic en el boton Add SSH key.

## Clonando el repositorio
17. Ingresar al repositorio que se clonará en GitHub
18. Clicar en el boton verde "Code" y seleccionar SSH
19. Copiar en el portapapeles la ruta git@github.com:saxtonv/cloud-computing.git
20. Abrir la terminal en la carpeta donde queremos clonar el repositorio
21. Ejecutar el comando `git clone git@github.com:saxtonv/cloud-computing.git`