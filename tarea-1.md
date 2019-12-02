# Instalacion de servicios basicos de ubuntu server
## Instalacion de apache2
Primero antes que nada es siempre recomendable hacer un update de los repositorio
![imagen update](capturas/tarea-1/Captura3.PNG)

A continuacion despues de actualizar los repositorios vamos a instalar el apache2
![imagen apache2](capturas/tarea-1/Captura4.PNG)

Ya hemos terminado la instalacion del apache, es bastante sencillo pero deberemos hacer cambios en el aws para que funcione el protocolo http/https

Para esto deberemos meternos en el panel de control y en la descripcion deberemos elegir el launch wizard
![imagen de launch-wizard](capturas/tarea-1/HTTP1.PNG)

A continuacion deberemos darle a editar y a continuacion añadiremos los servicios http y https
![imagen añadir protocolos](capturas/tarea-1/HTTP2.PNG)

## Instalar mySQL
primero pondremos este comando para que instalemos el mysql server con este comando
![primer paso mysql](capturas/tarea-1/Captura7.PNG)

y a continuacion pondremos el comando para configurar el servicio 
![configuracion de mysql](capturas/tarea-1/Captura6.PNG)

## Instalar phpmyadmin
Pondremos el siguiente comando para instalar

![instalacion phpmyadmin](capturas/tarea-1/Captura8.PNG)

ahora comenzaremos con los pasos de la instalacion

* primero aquí elegiremos apache **pulsando espacio** y cuando lo hayamos hecho le daremos a enter
![instalacion phpmyadmin 2](capturas/tarea-1/Captura9.PNG)

* seleccionaremos la opcion de configurar la base de datos
![instalacion phpmyadmin 3](capturas/tarea-1/Captura10.PNG)

* ahora nos toca elegir la contraseña, aquí se aplican las reglas de cuando has configurado el mysql
![instalacion phpmyadmin 4](capturas/tarea-1/Captura11.PNG)
* a continuacion elegiremos el metodo de conexion a la base de datos, en mi caso he elegido TCP/IP
![instalacion phpmyadmin 5](capturas/tarea-1/Captura12.PNG)
* en el siguiente paso elegiremos el host, en mi caso he elegido localhost
![instalacion phpmyadmin 6](capturas/tarea-1/Captura13.PNG)
* para este paso en un principio no deberemos cambiar el puerto
![instalacion phpmyadmin 7](capturas/tarea-1/Captura14.PNG)
* ahora elegiremos el nombre de la base de datos
![instalacion phpmyadmin 8](capturas/tarea-1/Captura15.PNG)
* Y por último el usuario del phpmyadmin
![instalacion phpmyadmin 9](capturas/tarea-1/Captura16.PNG)

al terminar todo esto podemos hacer una comprobacion de si hemos conseguido instalar con exito
![instalacion phpmyadmin 10](capturas/tarea-1/Captura17.PNG)

## Conexion SQL php

Por ultimo para crear la conexion entre SQL y ya lo tendriamos todo preparado para ponernos a trabajar
```
sudo apt install php libapache2-mod-php php-mysql
```


