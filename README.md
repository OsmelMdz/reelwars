# Curso Java: Consumir API, escribir archivos y manejar errores

Este repositorio contiene el proyecto **ReelWars**, desarrollado como parte del curso **"Java: Consumir API, escribir archivos y manejar errores"** impartido por **Bruno Darío Fernández Ellerbach** a través de **Alura Latam**.

Durante este curso, puse en práctica habilidades clave para el desarrollo de aplicaciones Java conectadas con APIs externas, procesamiento de respuestas en formato JSON, persistencia de datos en archivos locales y manejo robusto de excepciones.

## Descripción

En el proyecto **ReelWars**, el usuario puede ingresar un número correspondiente a una película del universo **Star Wars**, y el sistema consultará automáticamente los datos usando la **API SWAPI**. La información obtenida incluye título, episodio, texto inicial (opening crawl), director, productor y fecha de estreno. Una vez obtenida, dicha información se guarda como archivo `.json` de forma local para consulta futura.

Durante el desarrollo apliqué los siguientes conceptos clave:
- **Consumo de APIs HTTP**: Realicé peticiones `GET` utilizando la clase `HttpClient` de Java.
- **Procesamiento de JSON**: Utilicé la biblioteca **Gson** para deserializar los datos en un objeto `Pelicula`.
- **Escritura de archivos locales**: Guardé la información obtenida en archivos `.json` mediante `FileWriter`.
- **Manejo de errores**: Incorporé bloques `try-catch` para manejar errores de red, formato de número inválido y problemas de escritura.
- **Buenas prácticas de diseño**: Separé la lógica en clases como `Principal`, `ConsultaPelicula`, `GeneradorDeArchivo` y el modelo `Pelicula`.

## Tecnologías utilizadas
- **Java**: Lenguaje de programación utilizado para la creación del proyecto.
- **JDK 17.0.6**: Versión del Java Development Kit empleada.
- **IntelliJ IDEA**: IDE utilizado para el desarrollo del proyecto.
- **Gson**: Biblioteca externa usada para convertir datos JSON en objetos Java.
- **API SWAPI**: Servicio web gratuito que provee información sobre el universo de Star Wars.

## Requisitos
- Tener instalado [Java JDK 17.0.6](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html).
- IntelliJ IDEA o cualquier otro IDE compatible con Java.
- Conexión a internet para consultar la API de SWAPI.
- Biblioteca Gson descargada y añadida al classpath del proyecto (si no se usa Maven o Gradle).

## Cómo ejecutar el proyecto

1. Clona el repositorio en tu máquina local.
2. Abre el proyecto con IntelliJ IDEA.
3. Verifica que la biblioteca **Gson** esté añadida correctamente.
4. Ejecuta el archivo `Principal.java` como aplicación Java.
5. Ingresa el número de la película de Star Wars que deseas consultar (por ejemplo, 1).

> Nota: Si introduces un número inválido o inexistente, el programa lo detectará y mostrará un mensaje de error adecuado.

## Lo aprendido en este curso
- Realizar peticiones HTTP en Java con `HttpClient`.
- Convertir datos JSON a objetos Java con Gson.
- Persistir información en archivos `.json` localmente.
- Implementar manejo de excepciones para errores comunes en conexión, parseo y escritura.
- Diseñar un programa estructurado y extensible, reutilizando clases y aplicando POO.

## Instructor
**Bruno Darío Fernández Ellerbach**  
Ingeniero en Sistemas de Información, egresado de la UTN Mendoza, Argentina.  
Especializado en desarrollo de aplicaciones Android y docente en Alura desde 2020.  
LinkedIn: [Bruno Darío Fernández Ellerbach](https://www.linkedin.com/in/brunofernandezellerbach/)  
GitHub: [bfjeje](https://github.com/bfjeje)
