# Instalacion Node.js en un sistema linux  
Configuración de un sistema linux con node.js
  
## Activación del protocolo SSH (OPCIONAL) 
La activación del protocolo SSH se ejecuta mediante el uso del siguiente comando `sudo systemctl enable ssh`, tras esto, para poder conectarnos remotamente a nuestra raspberry deberemos ejecutar el comando `ifconfig` y nos mandará una serie de IPs, la que nosotros debemos usar es la wue está en el apartado *inet*

## Actualización de los paquetes
Tras habernos conectados por SSH mediante algún programa como **Putty**, debemos actualizar todos nuestros sistemas mediante el comando `sudo apt update` y `sudo apt full-upgrade` 
  
## Ver nuestra versión de node y npm
Para comprobar nuestra versión de node y de npm, debemos hacer uso de la función `-v`, por lo que deberemos ejecutar los comandos `node -v` y `npm -v`; probablemente os salga una versión de npm y node obsoleta, y como nosotros queremos la más reciente a continuación os explico como se descarga.
 
## Instalación de paquetes
Lo primero que debemos hacer uso del comando `curl -sL https://deb.nodesource.com/setup_14.x -o nodesource_setup.sh`. posteriormente debemos ejecutar los comandos `nano nodesource_setup.sh` y editar el archivo para que quede como el que adjunto a continuación:
```
SCRSUFFIX="_14.x"
NODENAME="Node.js 14.x" 
NODEREPO="node_14.x"
NODEPKG="nodejs"
```

## Instalación de node.js 
Debemos ejecutar el comando `sudo bash nodesource_setup.sh`, y posteriormente instalar los paquetes de node.js `sudo apt-get install -y nodejs`.

## Comprobando la instalación
Finalmente para comprobar que hemos descargado de forma correcta debemos ejecutar el comando `node -v` y `npm -v`

## No lo entendí... ¿Cómo puedo contactar contigo?
Puedes abrirme una **issue** desde aquí, o puedes contactarme a través de mi servidor de Discord o a través de mi usuario de Discord, `Chiquicalris#1337`

### Gracias por leer!
Agradecería que me apoyases dandome una estrella o siguiéndome, a continuación te dejo algunos links de utilidad:
✨ · *[Servidor de Discord](https://discord.gg/VPjePtWV6f)* 
🔌 · *[Mi bot de Discord](https://docs.foxybot.ga)* 

 
