# Portafolio-individual-Apps-Moviles-cancheito-Shamir_Erick
## Resumen Ejecutivo  

El proyecto **Cancheito** consiste en una aplicación móvil nativa en Kotlin que conecta postulantes y empleadores en el mercado laboral boliviano. El sistema permite a los postulantes registrarse, crear perfiles completos, subir su CV, buscar y postularse a ofertas laborales, mientras que los empleadores pueden publicar vacantes, gestionar postulaciones y acceder a los perfiles de los candidatos.  

Mi contribución se centró en dos ejes principales: liderazgo y desarrollo técnico. Asumí el rol de **Scrum Master**, coordinando las ceremonias ágiles y garantizando el cumplimiento de la metodología. Además, participé activamente como desarrollador, implementando historias como la **US-013 (Calificar empleador/postulante, posteriormente por un cambio dentro del sprint se volvio en la US-012)** y la **US-004 registro de empleador**, que son funcionalidades críticas para el MVP.  

De forma complementaria, también realicé pruebas exhaustivas en las funcionalidades implementadas por mis compañeros aceptando los cambios dentro de GitHub, asegurando la calidad del producto, mi participación directa en aproximadamente el **70 % de los sprints** permitió que el equipo alcanzara un progreso sostenido y mantuviera un nivel alto de compromiso y entrega.

## Contribuciones Técnicas  

### Tecnologías utilizadas  

### Frontend Móvil
- **Kotlin + Android Studio**  
- **Material Design 3 + Jetpack Compose**  
- **Coroutines**  

### Frontend Web
- **Next.js 14 + React 18**  
- **TypeScript + Tailwind CSS**  

### Backend & Database
- **Firebase Authentication (Email/Password + Google OAuth)**  
- **Cloud Firestore**  
- **Firebase Storage**  
- **Room Database (offline)**  

### Tools
- **Git + GitHub**  
- **Gradle Build System**  
- **APK Signing**  
- **Android Studio, Git/GitHub, Jira, Miro.**

### Contribuciones clave del código  

- **Implementación de la US-013 / US-012 (Calificar empleador y postulante):**  
  Desarrollo completo del flujo de calificación, incluyendo botones, navegación, persistencia de puntajes y sincronización en Firebase.  
  🔗 [Ver commit](https://github.com/Jhoel777ar/cancheito_app_preview/commit/0843eb9d65cc62a380d146ce5d393398ae04254c)  

- **Desarrollo de la US-004 (Registro de usuarios y validaciones):**  
  Implementación del registro de cuentas con correo/contraseña, validaciones de campos obligatorios y manejo de errores comunes en la creación de usuarios.  
  🔗 [Ver commit](https://github.com/Jhoel777ar/cancheito_app_preview/commit/fc112f8a4142a192668605cb29dc5ff90f22f4fb)  

- **Optimización en la integración con Firebase (Auth y Firestore):**  
  Ajustes en la lógica de autenticación, gestión de perfiles y almacenamiento de datos en la nube, garantizando mayor estabilidad y consistencia entre frontend y backend.  
  🔗 [Ver commit](https://github.com/Jhoel777ar/cancheito_app_preview/commit/b6a56136515280cc3e9197cc3521634735a76250)  


### Desafíos técnicos resueltos  

### Desafío 1: Sincronización Offline–Online
- **Problema:** Riesgo de pérdida de datos al usar la aplicación sin conexión.  
- **Solución:** Implementación de una **cola de operaciones** en **Room Database** con sincronización en segundo plano mediante **WorkManager**, garantizando la persistencia y posterior actualización en la nube.  
- **Aprendizaje:** Adopción de una **arquitectura offline-first**, comprensión profunda del manejo de estados de sincronización y resiliencia en entornos con conectividad limitada.  

### Desafío 2: Autenticación con Google
- **Problema:** Errores en la configuración de **SHA-1** y credenciales OAuth que impedían el inicio de sesión.  
- **Solución:** Generación y registro correctos de certificados, junto con la configuración adecuada del archivo **google-services.json** en Firebase Console.  
- **Aprendizaje:** Dominio del flujo de **OAuth 2.0**, mejores prácticas en la **gestión segura de credenciales** y fortalecimiento de la experiencia en integraciones con Firebase.  

### Desafío 3: Actualización en Tiempo Real del Panel Admin
- **Problema:** Los cambios en las colecciones no se reflejaban de forma inmediata en la vista del administrador.  
- **Solución:** Uso de **Firestore onSnapshot listeners** combinados con **React Context** para propagar los cambios en tiempo real a todos los componentes del panel.  
- **Aprendizaje:** Profundización en **state management avanzado** y en patrones de aplicaciones **colaborativas en tiempo real**, mejorando la fluidez de la experiencia de usuario.

### Servicios creados  
- `auth.service.ts`: Servicio para login, registro y persistencia de sesión.  
- `grades.service.ts`: Servicio para gestión y validación de calificaciones en perfiles.  

### Integraciones  
- **Firebase:** Autenticación con email y Google, Firestore para persistencia y Storage para CVs/fotos.  
- **APIs externas:** Integración con servicios de calendario/clima en pruebas exploratorias.  
- **Pruebas físicas:** Validación en dispositivos Android gama media, garantizando fluidez y usabilidad.  

---

## Aplicación de la Metodología Ágil  

- **Roles ejercidos:** Scrum Master, Desarrollador, Tester.  
- **Participación en ceremonias:** Facilitación de *Daily Scrums*, *Sprint Planning*, *Reviews* y *Retrospectives*.  
- **Métricas personales de contribución:**  
  - Participación en mayor al 70 % de sprints activos.  
  - Desarrollo de 3 historias críticas del backlog.  
  - Pruebas funcionales en +10 features de compañeros.  

---

## Desarrollo de Habilidades Blandas  

- **Comunicación:** Coordinación efectiva entre desarrolladores, resolución de dudas en reuniones y chat de equipo.  
- **Liderazgo:** Como Scrum Master, organicé los sprint plannings y mantuve la motivación del equipo.  
- **Resolución de problemas:** Intervine en bugs críticos de Firebase y en flujos de autenticación.  
- **Adaptabilidad:** Roté entre funciones de desarrollador, tester y líder ágil según lo requirió el sprint.  

---

## Artefactos y Evidencia  

### App Móvil
✅ Implementación de la **US-013 / US-012 (Calificar empleador y postulante)** → [Commit](https://github.com/Jhoel777ar/cancheito_app_preview/commit/0843eb9d65cc62a380d146ce5d393398ae04254c)  
✅ Desarrollo de la **US-004 (Registro de usuarios y validaciones)** → [Commit](https://github.com/Jhoel777ar/cancheito_app_preview/commit/fc112f8a4142a192668605cb29dc5ff90f22f4fb)  
✅ Ajustes en **Firebase Auth y Firestore** para la gestión de perfiles → [Commit](https://github.com/Jhoel777ar/cancheito_app_preview/commit/b6a56136515280cc3e9197cc3521634735a76250)  
✅ Capturas de la aplicación funcionando en **emulador y dispositivos físicos** (validación propia como tester)  

### Documentación y Testing
✅ Evidencia de pruebas de las funcionalidades implementadas por mis compañeros (rol de **tester**)  
✅ Documentación de avances en **User Stories** y definición de criterios de aceptación  
✅ Registro de mi participación como **Scrum Master** en ceremonias (Daily, Planning, Retrospectiva)  

### Código y Evidencia Técnica
✅ Fragmentos clave en `MisPostulacionesFragment.kt` y `DetallePostulanteFragment.kt` (flujo de calificaciones y postulaciones)  
✅ Configuración de **Firebase Authentication y Realtime Database** aplicada en mis historias  
✅ **APK firmado** probado y verificado con mis desarrollos en dispositivos físicos   

---

## Reflexión y Crecimiento Futuro  

- **Autoreflexión:** El proyecto me permitió afianzar mi dominio en Kotlin, Firebase y metodologías ágiles. Destaco el valor de liderar como Scrum Master mientras sigo siendo un desarrollador activo.  
- **Plan de crecimiento:** Mejorar mis habilidades en notificaciones push, almacenamiento local con SQLite y optimización de rendimiento.  
- **Impacto profesional:** Este proyecto fortaleció mi visión de combinar desarrollo técnico con liderazgo ágil, lo que será clave en futuros desafíos laborales.  

---

## Declaración de Compromiso de Aprendizaje (Día 20)  

### Habilidades técnicas (próximos 6 meses)  
1. Dominar el uso de **Capacitor plugins** para funcionalidades nativas.  
2. Implementar **SQLite/IndexedDB** para persistencia local en proyectos híbridos.  
3. Integrar **servicios RESTful externos** de forma robusta y escalable.  

### Prácticas ágiles  
1. Aplicar *Definition of Done* clara en cada entregable.  
2. Medir y mejorar *velocity* en futuros equipos.  
3. Implementar *retrospectivas* accionables con planes de mejora continua.  

### Colaboración  
1. Mejorar feedback constructivo en code reviews.  
2. Potenciar liderazgo compartido en ceremonias Scrum.  
3. Desarrollar empatía para fomentar un clima de equipo colaborativo.  

### Métricas de éxito  
- Alcanzar **85 %+ de cobertura en tests**.  
- Reducir bugs críticos en un **30 %** en siguientes proyectos.  
- Participar en **2 proyectos nuevos** aplicando prácticas ágiles mejoradas.  

### Socio de responsabilidad  
- **Compañero asignado:** [Luis Fernando Villca Mamani] (para dar seguimiento trimestral).  

### Fecha de revisión  
- **Dentro de 3 meses:** Evaluar avances y definir siguientes pasos.

## Contacto

**👤 Nombre:** Shamir Erick Condori Troche  
**👨‍💻 GitHub:** [SamStorm2003](https://github.com/SamStorm2003)  

---

### **Stark Storm**  
*"La verdadera fuerza de un equipo no está en el código que escribe, sino en la confianza que construye."*  

