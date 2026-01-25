# 🗺️ MappsApp

Una aplicación Android moderna desarrollada en Kotlin que integra Google Maps, autenticación de usuarios y base de datos en tiempo real con Supabase.

## 📋 Características

- **🗺️ Integración de Google Maps**: Visualización de mapas interactivos con soporte completo de Google Maps
- **📍 Geolocalización**: Servicios de ubicación en tiempo real
- **🔐 Autenticación**: Sistema completo de autenticación de usuarios con Supabase
- **💾 Base de datos en tiempo real**: Sincronización de datos con Supabase
- **📦 Almacenamiento**: Gestión de archivos con Supabase Storage
- **🎨 UI Moderna**: Interfaz construida con Jetpack Compose y Material3
- **🧭 Navegación**: Navegación fluida entre pantallas con Navigation Compose

## 🛠️ Tecnologías y Librerías

### Core
- **Kotlin** - Lenguaje de programación principal
- **Jetpack Compose** - Framework moderno de UI para Android
- **Material3** - Sistema de diseño de Google

### Mapas y Localización
- **Google Maps Compose** (v2.11.4) - Integración de mapas en Compose
- **Play Services Maps** (v19.2.0) - SDK de Google Maps
- **Play Services Location** (v21.3.0) - Servicios de ubicación

### Backend y Base de Datos
- **Supabase** (v3.1.4) - Backend as a Service
  - PostgREST - Base de datos
  - Auth - Autenticación
  - Storage - Almacenamiento de archivos
- **Ktor Client** (v3.1.2) - Cliente HTTP

### Otras Librerías
- **Coil** (v2.7.0) - Carga de imágenes
- **Kotlinx Serialization** - Serialización de datos JSON
- **Navigation Compose** - Navegación entre pantallas
- **Lifecycle ViewModel Compose** - Gestión del estado de la UI

## 📦 Requisitos

- **Android Studio**: Koala o superior
- **Kotlin**: 1.9+
- **SDK mínimo**: Android 7.0 (API 24)
- **SDK objetivo**: Android 14 (API 35)
- **JDK**: Java 11

## 🚀 Configuración del Proyecto

### 1. Clonar el repositorio

```bash
git clone https://github.com/daoudoudada/MappsApp.git
cd MappsApp
```

### 2. Configurar las API Keys

Crea un archivo `local.properties` en la raíz del proyecto con las siguientes claves:

```properties
supabaseUrl=TU_SUPABASE_URL
supabaseKey=TU_SUPABASE_ANON_KEY
```

### 3. Configurar Google Maps API

Crea/edita el archivo `secrets.properties` en la raíz del proyecto:

```properties
MAPS_API_KEY=TU_GOOGLE_MAPS_API_KEY
```

#### Obtener la API Key de Google Maps:

1. Ve a [Google Cloud Console](https://console.cloud.google.com/)
2. Crea un nuevo proyecto o selecciona uno existente
3. Habilita la **Maps SDK for Android**
4. Ve a "Credenciales" y crea una API Key
5. Restringe la API Key a tu aplicación Android

### 4. Configurar Supabase

1. Crea una cuenta en [Supabase](https://supabase.com/)
2. Crea un nuevo proyecto
3. Obtén la URL y la clave anónima desde la configuración del proyecto
4. Agrégalas al archivo `local.properties`

### 5. Compilar y Ejecutar

```bash
./gradlew assembleDebug
```

O ejecuta directamente desde Android Studio con el botón Run ▶️

## 📱 Estructura del Proyecto

```
MappsApp/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/mapsapp/
│   │   │   ├── res/
│   │   │   └── AndroidManifest.xml
│   │   └── ...
│   └── build.gradle.kts
├── gradle/
├── build.gradle.kts
├── settings.gradle.kts
├── local.properties (no incluido en git)
└── secrets.properties
```

## 🔒 Seguridad

⚠️ **Importante**: Nunca subas tus archivos `local.properties` o `secrets.properties` a GitHub. Estos archivos contienen información sensible y ya están incluidos en `.gitignore`.

## 🤝 Contribuir

Las contribuciones son bienvenidas. Para cambios importantes:

1. Haz un Fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la licencia que elijas especificar.

## 👤 Autor

**daoudoudada**
- GitHub: [@daoudoudada](https://github.com/daoudoudada)

## 🙏 Agradecimientos

- [Google Maps Platform](https://developers.google.com/maps)
- [Supabase](https://supabase.com/)
- [Jetpack Compose](https://developer.android.com/jetpack/compose)

---

⭐ ¡Si te gusta este proyecto, dale una estrella en GitHub!
```

