# Configurar servidor FTP
primero deberemos poner este comando para instalar el servicio vsftpd

si no funciona prueba a poner los siguientes comandos
```bash
sudo apt-get update

sudo apt-get upgrade
```
![instalacion vsftp](capturas/tarea-5/Captura1.PNG)

a continuacion usaremos estos comandos para que el servicio funcione
![iniciar servicio](capturas/tarea-5/Captura2.PNG)

en el siguiente paso crearemos usuarios para el servicio FTP
![usuarios](capturas/tarea-5/Captura3.PNG)

deberemos tener las siguientes lineas sin comentar:
![primera configuracion](capturas/tarea-5/ftpConf1.PNG)
![segunda configuracion](capturas/tarea-5/ftpConf2.PNG)
![tercera configuracion](capturas/tarea-5/ftpConf3.PNG)

para que nos funcione deberemos habilitar en nuestro servidor el puerto de entrada de ftp (el 21)
![puertos](capturas/tarea-5/captura4.PNG)

por ultimo reiniciaremos el servicio y ya podríamos usarlo
![puertos](capturas/tarea-5/captura5.PNG)