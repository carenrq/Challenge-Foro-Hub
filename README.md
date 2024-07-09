# Challenge ONE | Back End | Foro Alura 


### ¡Bienvenido al proyecto del desafío Foro Alura con Java y Spring! 

Este proyecto forma parte del desafío propuesto por Alura Latam en colaboración con Oracle para practicar habilidades de desarrollo back-end utilizando Java y Spring. A continuación, se detallan los pasos y tecnologías utilizadas para la implementación del proyecto.


## Tecnologías Utilizadas:

- [Eclipse](https://www.eclipse.org/)
- [MySql](https://www.mysql.com/)
- [Java](https://www.java.com/en/)
- [Spring Security](https://start.spring.io/)
- [Token JWT](https://jwt.io/)


## Funcionalidades de la API

### Registro de un Nuevo Tópico

La API cuenta con un endpoint para registrar nuevos tópicos utilizando solicitudes POST a la URI `/tópicos`. Los datos del tópico (título, mensaje, autor y curso) se envían en formato JSON y se validan antes de ser almacenados en la base de datos.

### Listado de Tópicos

Se ha implementado un endpoint GET para listar todos los tópicos disponibles en la URI `/tópicos`. La respuesta incluye detalles como título, mensaje, fecha de creación, estado, autor y curso en formato JSON.

### Detalle de Tópicos

La API proporciona un endpoint GET para obtener los detalles de un tópico específico a través de la URI `/tópicos/{id}`. Utilizamos `@PathVariable` para extraer el ID del tópico de la solicitud.

### Actualización de Tópico

Para actualizar la información de un tópico, se ha configurado un endpoint PUT en la URI `/tópicos/{id}`. Este endpoint valida los datos recibidos y asegura que el tópico existe en la base de datos antes de realizar la actualización.

### Eliminación de Tópico

La API también incluye un endpoint DELETE en la URI `/tópicos/{id}` para eliminar un tópico específico. Se verifica la existencia del tópico antes de proceder con su eliminación.

## Pruebas de la API

Se ha utilizado Postman para probar todas las funcionalidades de la API, asegurando que cada endpoint funcione correctamente y cumpla con los requisitos establecidos.

- [Postman](https://www.postman.com)

## Gestión de Código con GitHub

Todo el desarrollo del proyecto se ha gestionado utilizando Git y GitHub, manteniendo un repositorio actualizado y documentado con las nuevas características y mejoras.

## Autenticación y Seguridad

### Implementación de Spring Security

Se ha implementado Spring Security para garantizar que solo los usuarios autenticados puedan interactuar con la API. Se ha configurado una clase `SecurityConfigurations` para gestionar el acceso a través de solicitudes HTTP.

### Autenticación de Usuarios

Se ha desarrollado un controlador de autenticación que maneja las solicitudes de inicio de sesión, utilizando `AuthenticationManager` para validar las credenciales de los usuarios.

### Base de Datos de Usuarios

Se ha extendido la base de datos para incluir una tabla de usuarios, almacenando las credenciales de autenticación.

### Token JWT

Para aumentar la seguridad, se ha implementado el uso de tokens JWT para la autenticación. Se ha creado una clase `TokenService` para generar y validar tokens, y se han definido atributos de configuración en `application.properties`.

## Conclusión

El proyecto "Foro Hub" ha sido exitosamente desarrollado y configurado siguiendo las mejores prácticas de desarrollo con Spring Framework. Cada funcionalidad ha sido cuidadosamente implementada y probada, garantizando una aplicación robusta y segura.

### Recursos y Referencias

- [MySQL: desde la descarga e instalación hasta su primera tabla | Alura Cursos Online](https://www.aluracursos.com/blog/instalacion-mysql-windows)
- [Spring Boot 3: desenvolva uma API REST em Java](https://cursos.alura.com.br/course/spring-boot-3-desenvolva-api-rest-java/task/115970)
- [Spring Security Documentation](https://docs.spring.io/spring-security/reference/index.html)
- [JWT.IO](https://jwt.io/)

Para más detalles y acceso al código fuente, visita el repositorio en GitHub.
