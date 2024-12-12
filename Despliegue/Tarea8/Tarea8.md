# BIND MOUNTS


### 1. Crear la carpeta saludo y el archivo index.html

mkdir saludo
echo "<h1>HOLA SOY JUAN</h1>" > saludo/index.html

### 2. Crear y ejecutar los contenedores con Bind Mounts

docker run -d --name c1 -p 8181:80 -v $(pwd)/saludo:/var/www/html php:7.4-apache

docker run -d --name c2 -p 8282:80 -v $(pwd)/saludo:/var/www/html php:7.4-apache


### 3. Verificar la ejecución

docker ps

![Descripción de la imagen Tarea 8](1.jpg)