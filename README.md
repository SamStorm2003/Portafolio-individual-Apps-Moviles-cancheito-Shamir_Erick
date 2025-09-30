# Portafolio-individual-Apps-Moviles-cancheito-Shamir_Erick
## Resumen Ejecutivo  

El proyecto **Cancheito** consiste en una aplicación móvil nativa en Kotlin que conecta postulantes y empleadores en el mercado laboral boliviano. El sistema permite a los postulantes registrarse, crear perfiles completos, subir su CV, buscar y postularse a ofertas laborales, mientras que los empleadores pueden publicar vacantes, gestionar postulaciones y acceder a los perfiles de los candidatos.  

Mi contribución se centró en dos ejes principales: liderazgo y desarrollo técnico. Asumí el rol de **Scrum Master**, coordinando las ceremonias ágiles y garantizando el cumplimiento de la metodología. Además, participé activamente como desarrollador, implementando historias como la **US-013 (Calificar empleador/postulante, posteriormente por un cambio dentro del sprint se volvio en la US-012)** y la **US-004 registro de empleador**, que son funcionalidades críticas para el MVP.  

De forma complementaria, también realicé pruebas exhaustivas en las funcionalidades implementadas por mis compañeros aceptando los cambios dentro de GitHub, asegurando la calidad del producto, mi participación directa en aproximadamente el **70 % de los sprints** permitió que el equipo alcanzara un progreso sostenido y mantuviera un nivel alto de compromiso y entrega.

## Contribuciones Técnicas  

### Tecnologías utilizadas  
- **Frontend:** Kotlin, Android (API 24–34). 
- **Backend & Cloud:** Firebase (Auth, Firestore, Storage).  
- **Arquitectura:** MVC + Repository Pattern.  
- **Herramientas:** Android Studio, Git/GitHub, Jira, Miro.  

### Contribuciones clave del código  
- Implementación de la **US-013 / US-012 (Calificar empleador/postulante)** → [Commit Link 1].  
- Desarrollo de la **US-004 (Registro de usuarios y validaciones)** → [Commit Link 2].  
- Ajustes en integración con Firebase Auth y Firestore para manejo de perfiles → [Commit Link 3].  

### Desafíos técnicos resueltos  
- **Problema:** Inconsistencias en sincronización de datos entre nodos de Firestore y la UI dentro del perfil del empleador.  
  **Solución:** Implementación de `LiveData` y `coroutines` para manejo de asincronía.  
  **Aprendizaje:** La importancia de separar capas con MVVM para mejorar mantenibilidad.  

- **Problema:** Fallos en la puesta de calificacion luego de postular.
  **Solución:** Configuración correcta dentro de los fragments del empleador ya que ahi se guardaran las resenas.  
  **Aprendizaje:** Profundización dentro de todos los archivos que tengan que ver con el usuario empleador
