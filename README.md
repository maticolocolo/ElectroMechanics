# ⚙️ Electromechanics

## Descripción del proyecto

**Electromechanics** es una aplicación móvil Android orientada a la gestión de servicios de mantenimiento electromecánico, permitiendo conectar clientes y trabajadores mediante una plataforma digital.

El proyecto busca facilitar la administración de solicitudes, el seguimiento de servicios y la gestión de información mediante una aplicación móvil conectada a un backend y una base de datos Oracle.

## Tecnologías utilizadas

### Aplicación Android
- Kotlin
- Android Studio
- Jetpack Compose
- Material Design 3
- MVVM (Model-View-ViewModel)
- ViewModel
- StateFlow
- Room / SQLite
- Retrofit

### Backend
- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- API REST
- Maven

### Base de datos
- Oracle Cloud
- Oracle Database
- JDBC
- Hibernate ORM

### Herramientas de desarrollo
- Git
- GitHub
- Postman
- Android Studio
- Visual Studio Code

## Funcionalidades principales

### Módulo Cliente
- Inicio de sesión.
- Registro de solicitudes de mantenimiento.
- Ingreso de título y descripción de solicitudes.
- Consulta de solicitudes realizadas.
- Visualización del estado de las solicitudes.

### Módulo Trabajador
- Gestión de servicios asignados.
- Consulta de órdenes de trabajo.
- Registro de información de mantenimiento.
- Gestión de informes técnicos.
- Uso de funcionalidades de ubicación y cámara.

## Arquitectura del sistema

El proyecto utiliza una arquitectura basada en tres componentes principales:

1. **Aplicación Android:** desarrollada en Kotlin y Jetpack Compose.
2. **Backend:** desarrollado con Spring Boot, encargado de procesar las solicitudes y gestionar la comunicación mediante servicios REST.
3. **Base de datos:** Oracle Cloud, utilizada para almacenar la información del sistema.

### Flujo de comunicación

```text
        APLICACIÓN ANDROID
        Kotlin / Compose
               |
               |
            Retrofit
               |
               v
        BACKEND SPRING BOOT
             API REST
               |
               |
        Spring Data JPA
               |
               v
          ORACLE CLOUD
          BASE DE DATOS
```

## Backend y API REST

El backend permite gestionar la comunicación entre la aplicación Android y la base de datos.

Se utilizan servicios REST para operaciones como:

- Consultar solicitudes.
- Registrar nuevas solicitudes.
- Consultar información de servicios.
- Gestionar información de mantenimiento.

Las pruebas de comunicación y operaciones de la API se realizan mediante Postman.

## Base de datos

El sistema utiliza Oracle Cloud como plataforma de almacenamiento de información.

La conexión se realiza mediante JDBC y la persistencia de datos se gestiona utilizando Spring Data JPA e Hibernate.

## Instalación y ejecución

### Aplicación Android

1. Descargar o clonar el repositorio.
2. Abrir el proyecto desde Android Studio.
3. Esperar la sincronización de Gradle.
4. Configurar el acceso al backend.
5. Ejecutar la aplicación en un emulador o dispositivo Android.

### Backend

1. Abrir el proyecto backend.
2. Configurar las credenciales de conexión a Oracle.
3. Verificar la configuración de la base de datos.
4. Ejecutar el backend mediante Maven:

```bash
mvn spring-boot:run
```

El servidor estará disponible en el puerto configurado, normalmente:

```text
http://localhost:8080
```

### Conexión con dispositivo físico

Para ejecutar la aplicación desde un teléfono Android, se debe configurar la dirección IP local del computador donde se encuentra funcionando el backend.

## Pruebas realizadas

- Verificación de compilación Android.
- Pruebas de funcionamiento de la aplicación.
- Pruebas de endpoints mediante Postman.
- Pruebas de comunicación con el backend.
- Verificación de operaciones de solicitudes.
- Generación de APK en versión Release.
- Firma del APK de entrega.

## Versión de entrega

Se generó una versión de producción de la aplicación Android mediante Android Studio.

**Archivo:** `app-release.apk`

**Tipo de compilación:** Release

**Firma:** APK firmado.

## Documentación técnica

El proyecto contempla documentación técnica y diagramas que describen:

- Arquitectura general del sistema.
- Comunicación entre Android y backend.
- Funcionamiento de los componentes.
- Flujo de información.
- Integración con Oracle Cloud.

## Seguridad

- Las credenciales de Oracle deben mantenerse protegidas.
- No publicar contraseñas ni archivos Wallet.
- No subir claves privadas de firma al repositorio.
- Utilizar archivos de configuración seguros para las conexiones.

## Información académica

**Proyecto:** Electromechanics

**Área:** Desarrollo de aplicaciones móviles.

**Plataforma:** Android.

**Lenguaje principal:** Kotlin.

**Backend:** Spring Boot.

**Base de datos:** Oracle Cloud.

---

Desarrollado como proyecto académico de desarrollo de software.
