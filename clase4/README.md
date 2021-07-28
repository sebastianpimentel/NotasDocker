***Clase 4***
En este clase se manejo un archivo docker-compose con los siguientes comandos
**mkdir proxy** para crar un directorio
**vim docker-compose-yml** para crae y editar el archivo docker-compose
despues de ejecutar el anterior comando se abra dentro de la misma consola de comando una ventana donde debemos oprimir la tecla **i** para poder insertar las siguientes lineas
**version: '3'
services:
  web:
    image: dockercloud/hello-world
  lb:
    image: dockercloud/haproxy
    links:
      - web
    volumes:
      - /var/run/docker.sock:/var/run/docker.sock
    ports:
      - 80:80**
Debemos tener encuenta los espacios y saltos de linea para que no tengamos problema en la siguiente parte del proceso 
Una ves instalado o ejecutado lo anterior debemos levantar servicio con el comando 
**docker-compose up -d** para descarga la imagen y levantar el servicio 
y para poder ver la imgen colocamos nuestra ip con el puerto que le definimos anteriormente
Si combinamos los anteriores comandos ya vistos podemos reiniciar el servicio y entre muchas otras cosas que podemos hacer ya es cuestion y practica de cada persona meterse mas en el tema de docker para reforzar los conocimientos y conocer mas los comandos de docker

<img src="https://d33wubrfki0l68.cloudfront.net/e7a6759eb6232b4280b83b18aa255289d65e4b6e/7698a/images/logo.webp">