## Simple Java Application

Aplicacion simple de Java dockerizada

# Prerrequisitos

Ejecutar este proyecto es muy sencillo, sin embargo se debe tener en consideración las siguientes recomendaciones.

 - Tener instalado Maven y Java en el ambiente local, se debe declarar  sus variables de entorno.
 - Contar con una versión de JAVA 17 o superior
 - Tener disponible el puerto 9090

# Pasos para desplegar la aplicación 

 1. Se debe compilar las dependencia maven  dentro del directorio " quickstart-23.0.0.final\kitchensink-angularjs"  con el comando
	          `mvn clean package -DskipTests`
 2. Generar la imagen del contenedor :
    `docker buiild -t myapp . `
3.  Generar imagen del contenedor
`docker-compose up -d ` o  `docker compose up` 

## Acceder  al servidor 

 ###  Proxy nginx
 [http://localhost:9090/sing-up/](http://localhost:9090/sing-up/)
 
 ###  Directo al servidor web 
 [http://localhost:8080/kitchensink-angularjs/](http://localhost:8080/kitchensink-angularjs/)
