# M7-_EvaModulo

🗂️ Proyecto 1: Agenda de Empleados
📌 Descripción General
Aplicación web desarrollada con Spring Boot que permite la gestión completa de empleados mediante operaciones CRUD. El objetivo principal es administrar información personal y laboral de manera sencilla utilizando una interfaz web construida con Thymeleaf.

🔧 Tecnologías Utilizadas
Java 17

Spring Boot

Spring MVC

Spring Data JPA / Hibernate

Thymeleaf

MySQL

Maven

🧩 Funcionalidades Clave
Crear empleados

Listar empleados

Editar información existente

Eliminar empleados

Validaciones básicas de formulario

🛠️ Proceso de Creación
Configuración del proyecto con Spring Initializr.

Creación de la entidad Empleado y la base de datos en MySQL.

Implementación del repositorio JPA para facilitar el acceso a datos.

Desarrollo del controlador MVC para manejar rutas y vistas.

Construcción de vistas dinámicas con Thymeleaf.

Pruebas y ajustes en formularios.

⚠️ Retos Encontrados y Soluciones
1. Error de conexión a la base de datos
Problema: La aplicación no iniciaba por credenciales incorrectas o falta de creación de la BD.
Solución: Crear la base manualmente en MySQL y verificar propiedades en application.properties.

2. Validaciones en formularios
Problema: Algunos datos se enviaban vacíos.
Solución: Se aplicaron anotaciones como @NotBlank, @Email, etc.

3. Actualización incorrecta de empleados
Problema: El ID se regeneraba al editar.
Solución: Se respetó el ID existente en el método POST de actualización.

🗂️ Proyecto 2: Portafolio Final M6 (Gestión de Cursos y Usuarios)
📌 Descripción General
Proyecto final del módulo 6 que consiste en un sistema web con roles y autenticación, permitiendo que un administrador gestione cursos y que un empleado visualice los cursos asignados. Utiliza Spring Security para controlar accesos.

🔧 Tecnologías Utilizadas
Java 17

Spring Boot

Spring Security

Spring MVC

Spring Data JPA / Hibernate

Thymeleaf

MySQL

Maven

🧩 Funcionalidades Clave
Login con autenticación y autorización

Rol ADMIN: CRUD de cursos

Rol EMPLEADO: visualizar cursos

Seed de datos inicial con data.sql

Separación de vistas según rol del usuario

🛠️ Proceso de Creación
Estructura inicial del proyecto y configuración del pom.xml.

Creación de entidades: Usuario, Rol, Curso y Empleado.

Implementación del sistema de seguridad con Spring Security.

Desarrollo de controladores para admin y empleado.

Generación de plantillas con Thymeleaf diferenciadas por rol.

Inserción de datos iniciales en data.sql para pruebas.

Pruebas de autenticación y autorización.

⚠️ Retos Encontrados y Soluciones
1. Problemas al configurar Spring Security
Problema: El sistema no distinguía correctamente los roles.
Solución: Revisar el SecurityConfig.java, definir correctamente accesos con .hasRole("ADMIN") y .hasRole("EMPLEADO").

2. Redirección incorrecta después del login
Problema: Usuarios eran dirigidos a la misma página sin importar su rol.
Solución: Implementación de un SuccessHandler personalizado.

3. Conflictos en las plantillas Thymeleaf
Problema: Confusión entre rutas de vistas para admin y empleado.
Solución: Separar carpetas /admin y /empleado y ajustar rutas en los controladores.

📘 Conclusión General
 Ambos proyectos permitieron profundizar en el desarrollo de aplicaciones Java con Spring Boot, abordando temas como:

Arquitectura MVC

CRUD completos con JPA

Seguridad y roles con Spring Security

Integración con bases de datos relacionales

Desarrollo de vistas dinámicas con Thymeleaf

Gracias a estos proyectos se reforzaron buenas prácticas, resolución de errores comunes y comprensión de aplicaciones empresariales reales.

📎 Contacto
Julio Fonseca
Desarrollador Java Fullstack
LinkedIn: https://www.linkedin.com/in/julio-fonseca-82896b368
