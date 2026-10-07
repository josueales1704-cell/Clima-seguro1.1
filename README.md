# Clima Costa Perú 🇵🇪

Aplicación Android para consultar condiciones meteorológicas y recomendaciones de prevención para la costa del Perú.

## Funciones

- 🌦️ Consulta del clima actual mediante Open-Meteo.
- 📍 Ciudades: Pacasmayo, Trujillo, Chiclayo, Piura, Chimbote, Lima e Ica.
- 🔔 Notificaciones locales cuando se detectan condiciones meteorológicas relevantes.
- 🌊 Información sobre El Niño Costero y medidas de prevención.
- 🇵🇪 Acceso a información oficial de ENFEN.

> Las notificaciones de esta versión son generadas por la aplicación a partir de los datos meteorológicos consultados. No sustituyen las alertas oficiales de SENAMHI, INDECI o ENFEN.

## Compilar automáticamente con GitHub Actions

1. Crea un repositorio nuevo en GitHub.
2. Sube **todos los archivos y carpetas de este proyecto** a la rama `main`.
3. En GitHub entra a **Actions**.
4. Selecciona **Build APK**.
5. Cuando termine el proceso, abre la ejecución completada.
6. En **Artifacts**, descarga `ClimaCostaPeru-debug-apk`.
7. Dentro del ZIP encontrarás `app-debug.apk`.

El workflow también se ejecuta automáticamente cuando haces `push` a `main` o `master`. Puedes iniciarlo manualmente desde **Actions → Build APK → Run workflow**.

## Requisitos del proyecto

- Android Gradle Plugin 8.7.3
- compileSdk 35
- targetSdk 35
- minSdk 23
- Java 17 para la compilación de GitHub Actions

## Compilación local

Si tienes Gradle instalado, ejecuta:

```bash
gradle assembleDebug
```

El APK quedará en:

```text
app/build/outputs/apk/debug/app-debug.apk
```

## API meteorológica

La aplicación utiliza Open-Meteo y no necesita una API key para este uso básico.
