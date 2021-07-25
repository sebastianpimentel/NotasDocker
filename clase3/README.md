**clase 3 manejo de imagenes y contenedores**

![Docker](https://www.docker.com/sites/default/files/d8/styles/role_icon/public/2019-07/horizontal-logo-monochromatic-white.png?itok=SBlK2TGU)

**mkdir mi-primer-dockerfile**para empezar a crear un contenedor

**vim Dokerfile**  para crear un archivo dockerfile

**i** para insertar dentro del vim

**mkdir static-html-directory** para crear el directorio necesario que nos pide el Dockerfile

**vim index.html** ingresar el archivo

**cat index.html** para saber que tiene el archivo y mustra en pantalla

**docker image build -t some-content-nginx .** para construir la imagen

**docker image ls** para listar las imagenes

**docker image rmi nombre_de_la _imagen** para eliminar una imagen

**docker run --name some-nginx -d -p 8080:80 some-content-nginx** ejecuta el contenedor con some-nginx y que le envie a background

**docker stop some-nginx** para detener un contenedor 

**docker rm some-nginx** para eliminar el contenedor

para volver a levantar un servicio debe estar dentro de la 
carpeta **docker-compose up -d** para volver a levantar un contenedor o servicio

**docker container ls** para listar los contenedores 

**docker logs -f nombre_del_contenedor** para ver los logs de los contenedores

**curl -k localhost:8080** para reailzar un prueba

**docker exec -it nginx-final** para ingresar a un contenedor

**docker tag some-content-nginx sebastianpimentel/fedesoft-web** para preparar los archivos que vamos a subir al docker hub

**docker push sebastianpimentel/fedesoft-web** para subir los archivos a docker

**docker image rm sebastianpimentel:fedesoft-web** para eliminar un tag mal hecho

**docker pull sebastianpimentel/fedesoft-web** para descargar una imagen desde docker

con estos comandos podemos realizar el manejo de las imagenes y contenedores se debe seguir un orden y tener cuidado donde estamos trabajando para no cometer fallas.
