🚀 DemoApplication – Proyecto Spring Boot

Este proyecto es una aplicación básica construida con Java y Spring Boot, pensada como punto de partida para crear APIs REST, servicios backend o aplicaciones empresariales con el ecosistema Spring.

📁 Estructura del Proyecto
src/
 └── main/
      ├── java/
      │    └── com/techlab/demo/
      │         └── DemoApplication.java
      └── resources/
           ├── application.properties
           └── static/ (opcional)

🧩 Descripción

El proyecto contiene:

Una clase principal DemoApplication que inicia la aplicación mediante Spring Boot.

Dependencias y configuración estándar de Spring Boot (según tu pom.xml o build.gradle).

Preparado para agregar controladores, servicios, repositorios y entidades.

▶️ Ejecución del Proyecto
1. Requisitos

Java 17+ (o la versión definida en tu proyecto)

Maven o Gradle

IDE recomendado: IntelliJ IDEA, Eclipse o VS Code

2. Ejecutar desde consola
mvn spring-boot:run


o con Gradle

./gradlew bootRun

3. Ejecutar desde el IDE

Ejecuta la clase:

DemoApplication.java

🔧 Configuración

En el archivo:

src/main/resources/application.properties


puedes configurar:

Puerto del servidor

Datos de conexión a base de datos

Logs

Configuraciones personalizadas

Ejemplo:

server.port=8080
spring.application.name=demo-app

📡 Endpoints

Actualmente el proyecto no tiene controladores creados.
Para agregar uno simple:

@RestController
public class HelloController {

    @GetMapping("/hello")
    public String hello() {
        return "Hola desde Spring Boot!";
    }
}

🛠️ Tecnologías Utilizadas

Java

Spring Boot

Spring Web (opcional según dependencia)

Maven/Gradle
