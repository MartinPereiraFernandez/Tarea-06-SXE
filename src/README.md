# Academia Erasmus+
## Como se levanta?
Para ello necesitaremos saber que servicios vamos a usar, para esta ocasión hemos elegido:
###### Base de datos --> MariaDB  
###### Aplicación --> EspoCRM  
###### Herramienta para observar la BD --> Adminer  
Necesitamos tener el Docker con el Compose instalado, procederemos entonces con la instalación de EspoCRM:

### 1. Accederemos a la carpeta donde se encuentra el compose:  
cd rutaHaciaElArchivoDeDocker

### 2. Se creará el fichero con todas las variables y se rellenarán las 3 contraseñas necesarias:

En el .env debería aparecer algo así solo que se ocultan las contraseñas ya que es un example:
DB_ROOT_PASSWORD=  
DB_PASSWORD=  
ADMIN_PASSWORD=  

Esto se copiará al .env con el comando:  
###### cp .env.example .env

### 3. Con todo listo levantaremos la pila, lo que quiere decir que pondremos a funcionar los 3 servicios (mariadb, espocrm y adminer) con el siguiente comando:    
###### docker compose up -d

### 4. Comprobaremos que los servicios están levantados gracias al comando: 
###### docker compose ps 

### 5. Como últimos pasos accederemos a la aplicación con el enlace que nos entrega que en este caso es:  
###### http://localhost:8080 (usuario: "admin", password: ...)   
  
![image (1).png](../../../Descargas/image%20%281%29.png)  

Y comprobaremos que todo funciona correctamente:  
![Captura desde 2026-10-14 13-42-08.png](../../../Descargas/Captura%20desde%202026-10-14%2013-42-08.png)





