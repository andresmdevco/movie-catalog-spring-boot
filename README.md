# 🎬 Catálogo de Peliculas - Spring Boot

Aplicación web para gestionar un catálogo de películas, desarrollada con **Spring Framework** y **Spring Boot**.

Permite registrar películas con su género, actores protagonistas e imagen de portada, además de listar, editar y eliminar registros desde una interfaz web construida con Thymeleaf y Bootstrap.

## ✨ Funcionalidades

- Catálogo público paginado de películas (`/home`).
- Alta y edición de películas con validación de campos (`/pelicula`).
- Asociación de películas con **géneros** y **actores protagonistas** (relación muchos a muchos).
- Subida y previsualización de imagen de portada para cada película.
- Servido de archivos/imágenes mediante un endpoint dedicado (`/archivo`).
- Listado administrativo con opciones de edición y eliminación (`/listado`).
- Mensajes de retroalimentación (éxito/error) tras acciones como eliminar una película.

## 🛠️ Tecnologías

- **Java** + **Spring Boot**
- **Spring MVC** (controladores `@Controller` y `@RestController`)
- **Spring Data JPA** (repositorios `CrudRepository` / `JpaRepository`)
- **Thymeleaf** (plantillas y fragmentos reutilizables con `th:insert`)
- **Bootstrap 5** + **jQuery** (interfaz y validaciones en cliente)
- **Bean Validation** (`jakarta.validation`) para validar formularios
- Base de datos relacional (JPA) con datos de prueba precargados vía `import.sql`

## 🚀 Cómo ejecutar el proyecto

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/movies-catalog-spring-boot.git
   ```
2. Configura la base de datos en `src/main/resources/application.properties` según tu entorno.
3. Ejecuta la aplicación con Maven:
   ```bash
   ./mvnw spring-boot:run
   ```
4. Abre tu navegador en [http://localhost:8080/home](http://localhost:8080/home)

## 📚 Sobre este proyecto

Este proyecto fue desarrollado con fines de aprendizaje, como parte del curso de **Spring Framework y Spring Boot** de Código Facilito, con el objetivo de practicar el desarrollo de una aplicación web completa: modelado de entidades, relaciones JPA, manejo de archivos, validaciones y renderizado de vistas con Thymeleaf.

