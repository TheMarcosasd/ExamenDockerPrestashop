1. Lo primero seria instalar la imagen (usamos el comando *docker network create prestashop-net*, asi si no lo tenemos lo descarga).
2. Ahora usariamos *docker run -ti --name some-mysql --network prestashop-net -e MYSQL_ROOT_PASSWORD=admin -p 3307:3306 -d mysql:5.7*, con este codigo descargamos mysql y estariamos creando un contenedor para poder usarlo despues.
3. Ahora solo nos quedaria lanzar el contendor, para comprobar de manera basica que esta funcionando el prestashop (*docker run -d -p 8080:80 --name prestashop prestashop/prestashop*).
   