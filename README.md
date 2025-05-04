Ejercicio 1
Empezamos creando un nuevo repositorio privado en GitHub con el nombre examenUD5, configurado para trabajar mediante conexión SSH.

A continuación, generamos un proyecto Spring Boot en IntelliJ IDEA utilizando Maven como gestor de dependencias. Durante la creación del proyecto, seleccionamos las siguientes dependencias necesarias:

Spring Boot Starter Web

Spring Data JPA

H2 Database

Spring Boot DevTools

Dentro del proyecto, implementamos un controlador REST básico que devuelve un mensaje de bienvenida al acceder a la ruta http://localhost:8080/welcome.

Verificamos el funcionamiento correcto del proyecto ejecutándolo desde IntelliJ y accediendo a dicha URL en el navegador, donde se mostró el mensaje esperado.

Después, inicializamos el repositorio local con Git Bash desde Windows y configuramos la conexión SSH al repositorio remoto de GitHub. Añadimos todos los archivos, realizamos el primer commit y subimos el proyecto a la rama principal (main).

Ejercicio 2
Creamos una nueva rama a partir de main llamada feature/initial-setup.

En esta rama, eliminamos todas las dependencias del archivo pom.xml, dejando el bloque <dependencies> vacío. Subimos los cambios generados al repositorio.

A continuación, generamos una nueva rama a partir de feature/initial-setup con el nombre feature/add-dependencies.

En esta nueva rama, volvimos a añadir todas las dependencias necesarias dentro del archivo pom.xml, incluyendo:

spring-boot-starter-web

spring-boot-starter-data-jpa

h2

spring-boot-devtools

spring-boot-starter-test

Una vez realizadas las modificaciones, subimos los cambios a la rama correspondiente en GitHub.

Ejercicio 3
Creamos una nueva rama a partir de feature/add-dependencies con el nombre feature/compile-code.

Compilamos el proyecto utilizando Maven con el comando ./mvnw clean install desde Git Bash. La compilación fue exitosa, lo que se confirmó con el mensaje "BUILD SUCCESSFUL" mostrado en consola.

Por último, subimos los cambios a la nueva rama feature/compile-code en el repositorio remoto.

