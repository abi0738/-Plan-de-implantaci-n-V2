# 🎵 PLAN DE IMPLEMENTACIÓN PROFESIONAL

# 💃 DanceAshley – Plataforma de Clases de Baile en Línea

---

# 🌌 DESCRIPCIÓN GENERAL DEL PROYECTO

DanceAshley será una aplicación profesional desarrollada con Flutter y Dart orientada a la administración de clases de baile en línea con soporte multiplataforma para Android, IOS, Web y Windows.

La aplicación permitirá a estudiantes, instructores y administradores interactuar mediante una plataforma moderna, elegante y dinámica utilizando Firebase Authentication, Cloud Firestore y Firebase Storage como infraestructura principal en la nube.

El sistema estará enfocado en una experiencia visual premium inspirada en plataformas modernas de streaming y educación digital, incorporando dashboards administrativos, animaciones fluidas, widgets modernos y diseño UI/UX futurista.

---

# 🎯 OBJETIVO GENERAL

Desarrollar una aplicación multiplataforma moderna para administrar clases de baile en línea, permitiendo gestionar usuarios, cursos, clases, pagos, materiales y progreso académico mediante Flutter, Firebase y Provider.

---

# 🎯 OBJETIVOS ESPECÍFICOS

✅ Implementar autenticación segura mediante Firebase Authentication.
✅ Crear CRUD completo utilizando Cloud Firestore.
✅ Diseñar interfaces modernas y responsivas.
✅ Administrar usuarios, cursos y clases.
✅ Integrar reproducción multimedia para clases de baile.
✅ Implementar seguimiento de progreso estudiantil.
✅ Crear dashboards administrativos modernos.
✅ Generar APK funcional multiplataforma.
✅ Mantener una arquitectura limpia y escalable.
✅ Aplicar diseño UI/UX futurista y elegante.

---

# 🖥️ TECNOLOGÍAS A UTILIZAR

| Tecnología              | Función                   |
| ----------------------- | ------------------------- |
| Flutter                 | Framework multiplataforma |
| Dart                    | Lenguaje principal        |
| Firebase Authentication | Inicio de sesión          |
| Cloud Firestore         | Base de datos en la nube  |
| Firebase Storage        | Almacenamiento multimedia |
| Provider                | Gestión de estado         |
| VS Code / Antigravity   | Desarrollo                |
| GitHub                  | Control de versiones      |

---

# 🎨 SISTEMA DE DISEÑO UI/UX

## 🌈 PALETA DE COLORES PRINCIPAL

| Color             | Código  |
| ----------------- | ------- |
| ⚫ Negro Oscuro    | #0D0D0D |
| 🟣 Morado Neón    | #7B2FF7 |
| 🌸 Rosa Vibrante  | #F107A3 |
| 🔵 Azul Eléctrico | #00C2FF |
| ⚪ Blanco Suave    | #F5F5F5 |

---

# ✨ ESTILO VISUAL DE LA APLICACIÓN

✅ Diseño futurista premium
✅ Interfaz elegante tipo streaming
✅ Glassmorphism
✅ Cards modernas redondeadas
✅ Sombras suaves
✅ Gradientes neón modernos
✅ Navegación responsiva
✅ Animaciones fluidas
✅ Dashboard administrativo premium
✅ Compatible con modo móvil y escritorio

---

# 📱 PLATAFORMAS SOPORTADAS

✅ Android
✅ IOS
✅ Web
✅ Windows

---

# 🗂️ ESTRUCTURA PROFESIONAL DEL PROYECTO

```plaintext
danceashley/
│
├── android/
├── ios/
├── web/
├── windows/
├── assets/
│   ├── images/
│   ├── icons/
│   ├── animations/
│   └── videos/
│
├── lib/
│   ├── core/
│   ├── models/
│   ├── providers/
│   ├── services/
│   ├── screens/
│   ├── widgets/
│   ├── routes/
│   ├── themes/
│   ├── utils/
│   └── main.dart
│
├── test/
├── pubspec.yaml
└── README.md
```

---

# 🔐 SISTEMA DE AUTENTICACIÓN

La aplicación iniciará con:

1️⃣ Splash Screen animado
2️⃣ Pantalla Login
3️⃣ Registro de usuarios
4️⃣ Recuperar contraseña
5️⃣ Inicio de sesión con Google
6️⃣ Persistencia de sesión
7️⃣ Validaciones en tiempo real

---

# 🧠 GESTIÓN DE ESTADO

Se utilizará:

✅ Provider
✅ ChangeNotifier
✅ Arquitectura modular limpia

Providers principales:

* AuthProvider
* UserProvider
* ClassesProvider
* UIProvider

---

# 🔥 FIREBASE Y BASE DE DATOS

## 🔗 Servicios Firebase

| Servicio                | Función               |
| ----------------------- | --------------------- |
| Firebase Authentication | Login y registro      |
| Cloud Firestore         | CRUD y almacenamiento |
| Firebase Storage        | Videos e imágenes     |

⚠️ NO utilizar Analytics.
⚠️ NO utilizar configuración de producción.

---

# 🧩 ENTIDADES DEL SISTEMA

## 1️⃣ Usuario

* id_usuario
* nombre
* apellido
* email
* contraseña
* fecha_nacimiento
* telefono
* foto_perfil
* fecha_registro
* activo

---

## 2️⃣ Instructor

* id_instructor
* id_usuario
* biografia
* especialidad
* años_experiencia
* certificaciones
* calificacion_promedio

---

## 3️⃣ Categoría

* id_categoria
* nombre
* descripcion
* imagen

---

## 4️⃣ Curso

* id_curso
* id_instructor
* id_categoria
* titulo
* descripcion
* nivel
* precio
* duracion_horas
* imagen_portada
* fecha_creacion
* publicado

---

## 5️⃣ Clase

* id_clase
* id_curso
* titulo
* descripcion
* url_video
* duracion_minutos
* orden
* es_gratuita

---

## 6️⃣ Inscripción

* id_inscripcion
* id_usuario
* id_curso
* fecha_inscripcion
* fecha_vencimiento
* estado

---

## 7️⃣ Pago

* id_pago
* id_inscripcion
* monto
* metodo_pago
* referencia_transaccion
* fecha_pago
* estado

---

## 8️⃣ Reseña

* id_resena
* id_usuario
* id_curso
* calificacion
* comentario
* fecha_resena

---

## 9️⃣ Progreso

* id_progreso
* id_inscripcion
* id_clase
* completada
* fecha_completado
* tiempo_visto_segundos

---

## 🔟 Material de Clase

* id_material
* id_clase
* nombre
* tipo
* url_archivo
* fecha_subida

---

# ⚙️ FUNCIONALIDADES PRINCIPALES

## 👤 CRUD Usuarios

✅ Agregar usuarios
✅ Listar usuarios
✅ Actualizar usuarios
✅ Eliminar usuarios

---

## 🎓 CRUD Cursos

✅ Crear cursos
✅ Editar cursos
✅ Eliminar cursos
✅ Administrar niveles

---

## 🎥 CRUD Clases

✅ Crear clases
✅ Subir videos
✅ Editar clases
✅ Eliminar clases

---

## 💳 Pagos

✅ Registro de pagos
✅ Historial
✅ Estado de transacción

---

## ⭐ Reseñas

✅ Sistema de estrellas
✅ Comentarios

---

## 📈 Progreso

✅ Seguimiento de avance
✅ Tiempo visualizado
✅ Porcentaje completado

---

# 📦 DEPENDENCIAS PUBSPEC.YAML

## 🔹 Firebase

* firebase_core
* firebase_auth
* cloud_firestore
* firebase_storage

## 🔹 Estado

* provider

## 🔹 UI / UX

* google_fonts
* flutter_spinkit
* lottie
* animate_do
* font_awesome_flutter
* curved_navigation_bar
* salomon_bottom_bar

## 🔹 Multimedia

* video_player
* chewie
* cached_network_image
* image_picker

## 🔹 Utilidades

* shared_preferences
* intl
* connectivity_plus
* fluttertoast
* file_picker
* uuid
* url_launcher
* http

---

# 📅 FASES DE IMPLEMENTACIÓN

# 🔹 FASE 1 – CONFIGURACIÓN INICIAL

✅ Instalar Flutter SDK
✅ Configurar VS Code
✅ Instalar Firebase CLI
✅ Crear proyecto DanceAshley
✅ Vincular Firebase
✅ Configurar Android/Web/IOS/Windows

---

# 🔹 FASE 2 – DISEÑO UI/UX

✅ Crear wireframes
✅ Diseñar dashboard
✅ Diseñar login premium
✅ Crear navegación moderna
✅ Configurar colores y tipografías

---

# 🔹 FASE 3 – AUTENTICACIÓN

✅ Login
✅ Registro
✅ Recuperar contraseña
✅ Login con Google
✅ Persistencia de sesión

---

# 🔹 FASE 4 – FIRESTORE Y CRUD

✅ CRUD usuarios
✅ CRUD cursos
✅ CRUD clases
✅ CRUD materiales
✅ CRUD categorías

---

# 🔹 FASE 5 – MULTIMEDIA

✅ Videos
✅ Imágenes
✅ Material PDF
✅ Reproductor multimedia

---

# 🔹 FASE 6 – DASHBOARD ADMINISTRATIVO

✅ Estadísticas
✅ Panel administrador
✅ Gestión de usuarios
✅ Gestión de cursos

---

# 🔹 FASE 7 – TESTING

✅ Android
✅ Web
✅ IOS
✅ Windows
✅ Corrección de errores

---

# 🔹 FASE 8 – IMPLEMENTACIÓN FINAL

✅ Optimización
✅ APK Android
✅ Build Web
✅ Documentación
✅ Entrega final

---

# 🛡️ SEGURIDAD

✅ Validaciones de formularios
✅ Protección de rutas
✅ Control por roles
✅ Reglas Firestore
✅ Manejo de errores

---

# 🚀 RESULTADO FINAL ESPERADO

Al finalizar el proyecto se obtendrá una aplicación moderna, elegante y completamente funcional para la administración de clases de baile en línea, utilizando Flutter, Firebase y Provider con soporte multiplataforma y arquitectura profesional escalable.

## Prompt
DESARROLLAR UNA APLICACION PROFESIONAL MULTIPLATAFORMA UTILIZANDO FLUTTER Y DART PARA ADMINISTRAR UNA PLATAFORMA DE CLASES DE BAILE EN LINEA LLAMADA “DANCEASHLEY”, CON SOPORTE COMPLETO PARA ANDROID, IOS, WEB Y WINDOWS.

LA APLICACION DEBE TENER UNA INTERFAZ MODERNA, FUTURISTA, ELEGANTE Y RESPONSIVA, INSPIRADA EN PLATAFORMAS PREMIUM DE STREAMING Y EDUCACION DIGITAL. UTILIZAR UN DISEÑO UI/UX PROFESIONAL CON GLASSMORPHISM, ANIMACIONES SUAVES, CARDS REDONDEADAS, SOMBRAS MODERNAS, TRANSICIONES FLUIDAS Y COMPONENTES VISUALMENTE ATRACTIVOS.

🎨 PALETA DE COLORES OFICIAL:

* Negro oscuro → #0D0D0D
* Morado neón → #7B2FF7
* Rosa vibrante → #F107A3
* Azul eléctrico → #00C2FF
* Blanco suave → #F5F5F5

📌 CONFIGURACION GENERAL:

* Framework: Flutter
* Lenguaje: Dart
* Base de datos: Firebase Console + Cloud Firestore
* Autenticación: Firebase Authentication
* Gestión de estado: Provider
* NO utilizar Analytics
* NO utilizar modo producción
* Utilizar configuración estándar
* Proyecto completamente funcional y organizado profesionalmente

📁 ESTRUCTURA PROFESIONAL DEL PROYECTO:
ORGANIZAR TODO EL CODIGO DENTRO DE LA CARPETA LIB UTILIZANDO UNA ARQUITECTURA LIMPIA Y ESCALABLE.

ESTRUCTURA:

lib/
├── core/
├── models/
├── providers/
├── services/
├── screens/
├── widgets/
├── routes/
├── themes/
├── utils/
└── main.dart

🖥️ PLATAFORMAS:

* Android
* IOS
* Web
* Windows

🔐 SISTEMA DE AUTENTICACION:
LA APLICACION DEBE INICIAR CON:

1. Splash Screen animado
2. Pantalla Login moderna
3. Registro de usuarios
4. Recuperar contraseña
5. Inicio de sesión con Google
6. Persistencia de sesión

IMPLEMENTAR VALIDACIONES EN TIEMPO REAL Y MANEJO PROFESIONAL DE ERRORES.

👥 ROLES DEL SISTEMA:

* Administrador
* Instructor
* Estudiante

🔥 FIREBASE:
MI PROYECTO EN FIREBASE CONSOLE SE LLAMA:

* danceashley

MI BASE DE DATOS EN FIRESTORE SE LLAMA:

* danceashley

CONFIGURAR:

* Firebase Authentication
* Cloud Firestore
* Firebase Storage

NO UTILIZAR:

* Firebase Analytics
* Configuración Production

🧩 ENTIDADES Y TABLAS DEL SISTEMA:

1. Usuario

* id_usuario
* nombre
* apellido
* email
* contraseña
* fecha_nacimiento
* telefono
* foto_perfil
* fecha_registro
* activo

2. Instructor

* id_instructor
* id_usuario
* biografia
* especialidad
* años_experiencia
* certificaciones
* calificacion_promedio

3. Categoría

* id_categoria
* nombre
* descripcion
* imagen

4. Curso

* id_curso
* id_instructor
* id_categoria
* titulo
* descripcion
* nivel
* precio
* duracion_horas
* imagen_portada
* fecha_creacion
* publicado

5. Clase

* id_clase
* id_curso
* titulo
* descripcion
* url_video
* duracion_minutos
* orden
* es_gratuita

6. Inscripción

* id_inscripcion
* id_usuario
* id_curso
* fecha_inscripcion
* fecha_vencimiento
* estado

7. Pago

* id_pago
* id_inscripcion
* monto
* metodo_pago
* referencia_transaccion
* fecha_pago
* estado

8. Reseña

* id_resena
* id_usuario
* id_curso
* calificacion
* comentario
* fecha_resena

9. Progreso

* id_progreso
* id_inscripcion
* id_clase
* completada
* fecha_completado
* tiempo_visto_segundos

10. Material de Clase

* id_material
* id_clase
* nombre
* tipo
* url_archivo
* fecha_subida

⚙️ FUNCIONALIDADES PRINCIPALES:

👤 MODULO USUARIOS:

* CRUD completo de usuarios
* Agregar usuarios
* Listar usuarios
* Actualizar usuarios
* Eliminar usuarios
* Foto de perfil
* Roles y permisos

🎓 MODULO CURSOS:

* CRUD completo de cursos
* Crear cursos
* Editar cursos
* Eliminar cursos
* Categorías
* Niveles:

  * Principiante
  * Intermedio
  * Avanzado

🎥 MODULO CLASES:

* CRUD completo de clases
* Reproductor de video
* Videos almacenados en Firebase Storage
* Orden de reproducción
* Clases gratuitas

💳 MODULO PAGOS:

* Registro de pagos
* Historial
* Estados de pago

⭐ MODULO RESEÑAS:

* Sistema de estrellas
* Comentarios
* Calificaciones

📈 MODULO PROGRESO:

* Seguimiento por clase
* Porcentaje completado
* Tiempo visualizado

📂 MODULO MATERIALES:

* PDFs
* Audios
* Imágenes
* Links externos

🧠 GESTION DE ESTADO:
UTILIZAR PROVIDER COMO GESTOR PRINCIPAL.

CREAR:

* AuthProvider
* UserProvider
* CourseProvider
* ClassProvider
* ProgressProvider
* UIProvider

📦 DEPENDENCIAS NECESARIAS EN PUBSPEC.YAML:

FIREBASE:

* firebase_core
* firebase_auth
* cloud_firestore
* firebase_storage

GESTION DE ESTADO:

* provider

UI / UX:

* google_fonts
* flutter_spinkit
* lottie
* animate_do
* font_awesome_flutter
* curved_navigation_bar
* salomon_bottom_bar

MULTIMEDIA:

* video_player
* chewie
* cached_network_image
* image_picker

UTILIDADES:

* shared_preferences
* intl
* connectivity_plus
* fluttertoast
* file_picker
* uuid
* url_launcher
* http

📱 PANTALLAS A IMPLEMENTAR:

1. Splash Screen
2. Login
3. Registro
4. Recuperar contraseña
5. Dashboard principal
6. CRUD usuarios
7. CRUD cursos
8. CRUD clases
9. Detalle del curso
10. Reproductor de video
11. Perfil usuario
12. Estadísticas
13. Configuración
14. Pantalla de pagos
15. Seguimiento de progreso

📌 REQUISITOS IMPORTANTES:

* TODO EL PROYECTO DEBE SER COMPLETAMENTE FUNCIONAL
* GENERAR CODIGO LIMPIO Y DOCUMENTADO
* IMPLEMENTAR RESPONSIVE DESIGN
* UTILIZAR WIDGETS MODERNOS Y REUTILIZABLES
* CREAR NAVEGACION MODERNA
* IMPLEMENTAR BUENAS PRACTICAS DE FLUTTER
* UTILIZAR FIRESTORE COMO BASE DE DATOS PRINCIPAL
* CONFIGURAR FIREBASE CORRECTAMENTE PARA TODAS LAS PLATAFORMAS
* PREPARAR APK FUNCIONAL PARA ANDROID
* MANTENER ARQUITECTURA ESCALABLE

🚀 ANTES DE GENERAR CODIGO:

1. MOSTRAR PLAN DE IMPLEMENTACION COMPLETO
2. MOSTRAR ESTRUCTURA DE CARPETAS
3. EXPLICAR DEPENDENCIAS
4. EXPLICAR FLUJO DE NAVEGACION
5. EXPLICAR CONFIGURACION FIREBASE
6. DESPUES GENERAR EL CODIGO MODULO POR MODULO


