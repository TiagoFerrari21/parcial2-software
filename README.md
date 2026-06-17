# Parcial 2 - Software

**Nombre:** Tiago Ferrari
**Fecha:** 17 de junio de 2026
**Descripción:** Repositorio creado para el segundo parcial. Contiene una página web estática básica (HTML) que se sirve a través de un contenedor Docker utilizando Nginx, con el historial de cambios gestionado mediante Git.


## Pasos para la Instalación y Despliegue Local

### 1. Clonar el repositorio
Abre una terminal o consola de comandos y ejecuta:

Navega hacia la carpeta raíz del proyecto: cd parcial2-software

### 2. Construcción de la Imagen Docker

Para crear la imagen con el archivo HTML y la configuración de Nginx, ejecuta el siguiente comando en la raíz del proyecto (donde se encuentra el archivo Dockerfile): docker build -t imagen-parcial .

### 3. Ejecución del Contenedor

Para levantar el servidor web y asignarle un puerto accesible, ejecuta: docker run -d -p 8080:80 --name contenedor-parcial imagen-parcial

### 4. Acceso a la Aplicación

Una vez que el contenedor esté corriendo de fondo, abre tu navegador web preferido (Chrome, Edge, Firefox, etc.) e ingresa a la siguiente dirección: http://localhost:8080