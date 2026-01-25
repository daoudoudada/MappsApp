# Mapp APP

Descripción breve
Proyecto Android multiplataforma de ejemplo desarrollado con Kotlin y Java, construido con Gradle. Incluye integración con Supabase (Autenticación , Storage , Cámara, Location permissition).

## Tecnologías
- Kotlin
- Java
- Gradle
- Android SDK
- Supabase (Auth, Postgres, Realtime, Storage)
- OkHttp / Ktor (cliente HTTP)
- kotlinx\-serialization
- Coroutines
- Jetpack (ViewModel, LiveData / Flow)

## Requisitos
- Windows 10/11
- `Android Studio Otter 3 Feature Drop | 2025.2.3`
- JDK 11+ (o la versión indicada en `gradle.properties`)
- Android SDK (API level según `app/build.gradle`)
- Emulador o dispositivo físico con `adb` en `PATH`
- Cuenta y proyecto en Supabase

## Estructura principal
- `app/` \- módulo principal de la aplicación
- `app/src/main/java` \- código Kotlin/Java
- `app/src/test` \- tests unitarios
- `app/src/androidTest` \- tests instrumentados
- `app/build.gradle` \- dependencias del módulo
- `settings.gradle` \- módulos incluidos

## Instalación rápida
1. Clonar el repositorio:
   - `git clone <url-del-repositorio>`
2. Abrir el proyecto en `Android Studio Otter 3 Feature Drop | 2025.2.3`.
3. Agregar variables privadas en `local.properties` (no commitear).
4. Dejar que Gradle sincronice dependencias.

## Configuración de Supabase
1. Crear un proyecto en https://supabase.com y obtener:
   - `SUPABASE_URL` (ej.: `https://<proyecto>.supabase.co`)
   - `SUPABASE_ANON_KEY` (y/o `SERVICE_ROLE_KEY` si aplica)
2. En la consola de Supabase: habilitar proveedores de Auth y crear buckets en Storage según necesidad.
3. Añadir en `local.properties` (no subir al repo):

