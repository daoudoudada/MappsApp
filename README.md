# P3 Maps App

App Android hecha en **Kotlin** que combina **mapas**, **marcadores**, **cámara** y un backend con **Supabase** (base de datos, almacenamiento y autenticación). La idea principal es poder iniciar sesión, crear/guardar información y verla en el mapa.

## Funciones
- **Mapa interactivo** (zoom, mover, etc.)
- **Añadir marcadores** en el mapa
- **Guardar marcadores/datos** en la nube con **Supabase (Database)**
- **Autenticación** con **Supabase Auth** (registro / inicio de sesión / cierre de sesión)
- **Storage** con **Supabase Storage** (subida/gestión de imágenes o archivos)
- **Cámara**: tomar fotos desde la app (por ejemplo, asociarlas a un marcador)
- (Opcional según configuración) **Ubicación** del usuario con permisos

## Tecnologías
- Kotlin + Android SDK
- Supabase:
  - **Auth**
  - **Database**
  - **Storage**

## Requisitos
- Android Studio
- SDK de Android
- Dispositivo físico o emulador
- Proyecto/configuración de Supabase (URL y anon key)

## Configuración (Supabase)
1. Crea un proyecto en Supabase.
2. Configura:
   - Tablas en **Database** (por ejemplo, `markers` o similar)
   - Buckets en **Storage** (por ejemplo, `images`)
   - Proveedor(es) en **Auth**
3. Añade en el proyecto Android tus credenciales (URL y `anon key`) donde corresponda.

> Consejo: no subas claves sensibles al repositorio si el proyecto se hace público.

## Permisos
Según lo que use tu app, puede pedir:
- **Internet**
- **Ubicación** (fine/coarse)
- **Cámara**
- (En versiones recientes) permisos de lectura/escritura de imágenes si aplica

## Cómo ejecutar
1. Clona o descarga el repo.
2. Ábrelo en **Android Studio**.
3. Sincroniza Gradle.
4. Configura las credenciales de **Supabase**.
5. Ejecuta en emulador o móvil.

## Estructura (orientativa)
- `app/src/main/java/...` lógica de la app
- `app/src/main/res/...` vistas y recursos
- `AndroidManifest.xml` permisos y configuración
