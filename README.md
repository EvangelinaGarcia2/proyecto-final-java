Proyecto Java - API de Productos

Este proyecto es una aplicación Java desarrollada con Spring Boot que expone una API REST para gestionar productos. Incluye operaciones CRUD (crear, leer, actualizar y eliminar productos).

Tecnologías utilizadas

Java 21

Spring Boot 3.x

Spring Web

Spring Data JPA

Hibernate

MySQL (o base de datos configurada en application.properties)

Lombok para reducir código boilerplate
📁 Estructura del Proyecto
src/
 └── main/
      ├── java/com/techlab/demo/
           ├── controller
                 └── ProductController.java
           ├── entity
                 └── Product.java
           ├── repository
                 └── ProductRepository.java
           ├── service
                 └── ProductService.java
            ├── utils
                 └── StringUtils.java
           └── DemoApplication.java
      │         └── DemoApplication.java
      └── resources/
           ├── application.yaml
           └── products.sql

🧩 Descripción

El proyecto contiene:

Una clase principal DemoApplication que inicia la aplicación mediante Spring Boot.

Dependencias y configuración estándar de Spring Boot (según tu pom.xml o build.gradle).

Preparado para agregar controladores, servicios, repositorios y entidades.

📦 Modelo: Product

Representa un producto dentro del sistema.

Atributos:

Long id

String nombre

double precio

String descripcion

String categoria

🌐 Endpoints de la API

Método	Endpoint	Descripción
GET	/products	Lista todos los productos
GET	/products/{id}	Obtiene un producto por su ID
POST	/products	Crea un nuevo producto
PUT	/products/{id}	Actualiza un producto existente
DELETE	/products/{id}	Elimina un producto
