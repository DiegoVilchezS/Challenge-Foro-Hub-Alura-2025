# 🚀 Foro Hub - Challenge Backend Alura


**Foro Hub** es una API REST profesional desarrollada para gestionar los tópicos de un foro de discusión. Este proyecto forma parte del Challenge de Backend de Alura Latam y pone en práctica conocimientos avanzados de arquitectura de software, seguridad y persistencia.

---

## 🛠️ Características Técnicas

* **CRUD Completo**: Gestión total de tópicos (Crear, Listar con paginación, Actualizar y Eliminar).
* **Seguridad JWT**: Implementación de **Spring Security** con autenticación **Stateless** mediante JSON Web Tokens.
* **Cifrado BCrypt**: Hashing de contraseñas para garantizar la privacidad de los usuarios.
* **Documentación Interactiva**: Interfaz de **Swagger UI** para visualizar y probar los endpoints.
* **Migraciones con Flyway**: Gestión automatizada del esquema de la base de datos MySQL.
* **Validaciones**: Reglas de negocio aseguradas mediante `Bean Validation`.

---

## ⚙️ Requisitos e Instalación

### 1. Requisitos previos
* **JDK 17** o superior.
* **Maven** (incluido en el proyecto mediante `mvnw`).
* **MySQL 8.0** instalado y corriendo


## 📂 Estructura del Proyecto
controller: Definición de los recursos y controladores de la API.

domain: Entidades del modelo de negocio, Repositorios JPA y DTOs (Data Transfer Objects).

infra: Configuraciones de seguridad JWT, filtros de autenticación y manejo global de errores.

## 👨‍💻 Autor
Diego Vilchez Estudiante de Ingeniería de Sistemas e Informática – Universidad Tecnológica del Perú.

