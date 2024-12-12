docker run --name ubuntu -d ubuntu:18.04

### Salir del contenedor y comprobar que se ha parado

docker stop ubuntu

### Para comprobar que el contenedor se ha detenido, ejecuta:
docker ps -a

### Rearrancar el contenedor y comprobar que está funcionando

docker start ubuntu

### Para comprobar que está funcionando, ejecuta nuevamente:
docker ps

### Mostrar el fichero /etc/os-release sin entrar en el contenedor

docker exec ubuntu cat /etc/os-release

![Descripción de la imagen Tarea 3](1.jpg)