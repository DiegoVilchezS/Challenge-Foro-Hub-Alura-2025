🚀 Foro Hub - Challenge Backend Alura
Foro Hub es una API REST robusta desarrollada como parte del Challenge de Alura Latam. El objetivo principal es replicar el funcionamiento backend de un foro de discusión, permitiendo la gestión completa de tópicos, usuarios y seguridad.

🛠️ Características Técnicas
CRUD Completo de Tópicos: Creación, listado (con paginación y ordenamiento), actualización y eliminación física/lógica.

Seguridad Avanzada: Implementación de Spring Security con autenticación Stateless mediante JSON Web Tokens (JWT).

Cifrado de Datos: Almacenamiento seguro de contraseñas utilizando el algoritmo de hashing BCrypt.

Persistencia y Migraciones: Gestión de base de datos MySQL con Spring Data JPA y control de versiones de esquema con Flyway.

Documentación Automatizada: Interfaz interactiva generada con SpringDoc / Swagger UI.

Manejo de Excepciones: Sistema centralizado de tratamiento de errores para devolver códigos HTTP precisos (404 Not Found, 400 Bad Request, etc.).

⚙️ Requisitos e Instalación
1. Requisitos previos
JDK 17 o superior.

Maven 3.x.

MySQL 8.0.

2. Configuración de la Base de Datos
Accede a tu terminal de MySQL o Workbench y ejecuta:

SQL
CREATE DATABASE foro_hub_api;
Las tablas se crearán automáticamente al iniciar la aplicación gracias a Flyway.

3. Configuración del Entorno
Edita el archivo src/main/resources/application.properties con tus credenciales:

Properties
spring.datasource.url=jdbc:mysql://localhost/foro_hub_api
spring.datasource.username=TU_USUARIO
spring.datasource.password=TU_CONTRASEÑA

# Secreto para la firma de los Tokens JWT
api.security.secret=${JWT_SECRET:mi_secreto_super_seguro_12345}
📖 Documentación de la API (Swagger)
La API cuenta con una interfaz de Swagger para probar los endpoints directamente desde el navegador.

Ruta de acceso: http://localhost:8080/swagger-ui.html

Flujo de uso:
Realizar un POST a /login con las credenciales de usuario.

Copiar el jwtToken recibido.

Hacer clic en el botón "Authorize" de Swagger, escribir Bearer  seguido del token y autorizar.

📂 Estructura del Proyecto
controller: Endpoints de la API.

domain: Entidades JPA, Repositorios y DTOs (Data Transfer Objects).

infra: Configuraciones de Seguridad, Filtros JWT y Tratamiento de Errores.

👨‍💻 Autor
Diego Vilchez Estudiante de Ingeniería de Sistemas e Informática – Universidad Tecnológica del Perú (UTP, Sede Piura).

Apasionado por el desarrollo Backend y la ciberseguridad.
