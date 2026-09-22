# Diagrama de casos de uso del sistema Identipat IA

El diagrama presenta únicamente los siete casos de uso definidos para Identipat IA. Las actividades descritas dentro de cada flujo no se modelan como casos de uso adicionales.

```mermaid
flowchart LR
    visitante["Visitante"]
    administrador["Administrador"]

    subgraph sistema["Sistema Identipat IA"]
        direction TB

        acceso(["01. Acceso al sistema"])
        inicioSesion(["02. Inicio de sesión"])
        registro(["03. Registro de información personal"])
        prediccion(["04. Predicción de la modalidad de protección"])
        cambioContrasena(["05. Cambio de contraseña del administrador"])
        registroPredicciones(["06. Descarga del registro de predicciones"])
        actualizarUsuario(["07. Actualización de información personal"])
    end

    visitante --- acceso
    visitante --- registro
    visitante --- prediccion

    administrador --- inicioSesion
    administrador --- cambioContrasena
    administrador --- registroPredicciones
    administrador --- actualizarUsuario

    acceso -. "flujo alternativo: no registrado" .-> registro
    registro -. "permite acceder después del registro" .-> prediccion
    acceso -. "permite continuar al formulario" .-> prediccion
    inicioSesion -. "precondición de administrador" .-> cambioContrasena
    inicioSesion -. "precondición de administrador" .-> registroPredicciones
    inicioSesion -. "precondición de administrador" .-> actualizarUsuario

    classDef actor fill:#f4f1ea,stroke:#4b5563,stroke-width:2px,color:#111827
    classDef usecase fill:#e7f0f7,stroke:#245b78,stroke-width:1.5px,color:#102a43
    classDef boundary fill:#ffffff,stroke:#6b7280,stroke-width:1.5px,color:#111827

    class visitante,administrador actor
    class acceso,inicioSesion,registro,prediccion,cambioContrasena,registroPredicciones,actualizarUsuario usecase
    class sistema boundary
```

## Relaciones principales

- El `visitante` puede acceder al sistema, registrar su información personal y realizar una predicción.
- El `administrador` debe iniciar sesión para utilizar las funciones administrativas.
- El caso 01 redirige al caso 03 cuando el visitante no está registrado y permite continuar al caso 04 cuando el usuario está registrado.
- El caso 03 permite acceder al caso 04 después de completar el registro correctamente.
- Los casos 05, 06 y 07 requieren que el administrador haya completado el caso 02.
- No se representan relaciones `<<include>>` entre los siete casos, porque las validaciones, consentimientos, procesamiento, búsquedas y generación de archivos son pasos internos de sus respectivos flujos, no casos de uso independientes definidos por el sistema.
- Los flujos alternativos, como datos inválidos, usuario no encontrado o consentimiento revocado, se mantienen dentro de la especificación de cada caso.
