Parcial 2 - API RESTful con Spring Boot
Este proyecto corresponde al desarrollo del Parcial 2 sobre API RESTful utilizando Spring Boot 3+. Implementa un CRUD de productos, internacionalización, endpoints reactivos con WebFlux y pruebas con JUnit y StepVerifier.

 Requisitos Previos
Antes de ejecutar este proyecto, asegúrate de tener instalado:

Java 17 o superior
Maven 3.8+
Spring Boot 3+
IntelliJ IDEA (o cualquier otro IDE compatible con Spring Boot)
Postman (para probar los endpoints)
Git (para gestionar versiones y subir el código al repositorio)
 Instalación y Configuración
1️ Clonar el Repositorio
Ejecuta el siguiente comando en la terminal para clonar el proyecto:

sh
Copiar
Editar
git clone https://github.com/JorgeMario-V/Parcial2.git
2️ Importar el Proyecto en IntelliJ
Abre IntelliJ IDEA.
Selecciona File → Open.
Busca la carpeta del proyecto clonado y ábrela.
Espera a que Maven descargue las dependencias automáticamente.
3️ Configurar el Archivo application.properties
El archivo src/main/resources/application.properties ya viene preconfigurado para ejecutar la API correctamente.

4️ Ejecutar la Aplicación
En IntelliJ, abre la clase principal del proyecto (Parcial2Application.java).
Haz clic derecho y selecciona Run 'Parcial2Application'.
Si prefieres usar la terminal, ejecuta:

sh
Copiar
Editar
mvn spring-boot:run
 Endpoints de la API
1️ Endpoint de Saludo
GET /api/saludo
Respuesta: "¡Hola, API RESTful!"
Internacionalización (i18n)
GET /api/saludo?lang=es → "¡Hola, API RESTful en Español!"
GET /api/saludo?lang=en → "Hello, RESTful API in English!"
2️ CRUD de Productos
POST /api/productos → Agregar un producto.
GET /api/productos → Listar todos los productos.
GET /api/productos/{id} → Obtener un producto por ID.
PUT /api/productos/{id} → Actualizar un producto.
DELETE /api/productos/{id} → Eliminar un producto.
3️Endpoint Reactivo con WebFlux
GET /api/productos → Devuelve una lista de productos en formato reactivo con Flux.
 Pruebas Automatizadas
Para ejecutar las pruebas con JUnit y StepVerifier, usa el siguiente comando en la terminal dentro del proyecto:

sh
Copiar
Editar
mvn test
 Subir Cambios al Repositorio GitHub
Si realizas modificaciones y deseas subirlas a GitHub, ejecuta los siguientes comandos en la terminal de IntelliJ:

sh
Copiar
Editar
git add .
git commit -m "Actualización del código del parcial"
git push origin main
📌 Capturas de Pruebas en Postman y JUnit
Las capturas de pantalla de las pruebas realizadas en Postman y JUnit se encuentran en la carpeta /screenshots del repositorio.

📌 Enlace al Repositorio GitHub
https://github.com/JorgeMario-V/Parcial2.git
