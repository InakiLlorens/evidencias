# Creacion de virtualhosts

Primero crearemos los registros DNS (como en la tarea anterior)

en este caso crearemos uno de cliente y otro de server
![crear registros](capturas/tarea-4/Captura1.PNG)

a continuacion crearemos 2 carpetas, una de cliente y otra de servidor (con sus respectivos index)
![crear carpetas](capturas/tarea-4/Captura2.PNG)

despues debemos darle los permisos necesarios a la carpeta
![permisos](capturas/tarea-4/Captura3.PNG)

en el siguiente paso crearemos copias 
![crear archivos conf](capturas/tarea-4/Captura4.PNG)

ahora deberemos editar cada archivo con el servername adecuado (el del registro DNS) y cambiar el documentroot a la carpeta *que en este ejemplo es la de cliente*
![editar archivos conf](capturas/tarea-4/Captura5.PNG)

despues de realizar estos pasos deberemos habilitar dicha configuración con el siguiente comando

```sh
sudo a2ensite cliente.conf
```
y por ultimo nos saldría que usemos este comando para reiniciar el servicio y ya podríamos trabajar con el virtualhost
```sh
sudo systemctl restart apache2
```

![crear archivos conf](capturas/tarea-4/Captura6.PNG)