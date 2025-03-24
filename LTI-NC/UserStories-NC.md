# User Stories

## Historia de Usuario: Base de Datos Centralizada de Candidatos

Título: Base de Datos Centralizada de Candidatos

Como reclutador,
quiero tener una base de datos centralizada de candidatos,
para que pueda acceder fácilmente a todos los perfiles, realizar búsquedas eficientes y mantener un repositorio organizado de toda la documentación relacionada con los aspirantes.

### Descripción

Esta funcionalidad proporcionará un sistema de almacenamiento centralizado para todos los datos de los candidatos que interactúan con el proceso de selección. La base de datos permitirá organizar, buscar, filtrar y gestionar toda la información relacionada con los candidatos, desde sus datos personales y currículums hasta documentos adicionales y registros históricos de sus interacciones con la empresa. Esta estructura centralizada servirá como fundamento para múltiples funcionalidades del ATS.

### Prioridad

Alta

### Story points

13

### Estimación
| Metodología | Valoración | Significado |
| --- | --- | --- |
| Fibonacci | 13  | Tarea compleja que requiere análisis y diseño detallado |
| Planning Poker | 13  | Consenso del equipo sobre complejidad alta |
| Talla de camiseta | XL  | Esfuerzo considerable, requiere un sprint completo |


### Asignado a

* Backend (principal)
* Arquitecto de datos
* Especialista en seguridad

### Etiquetas

* Core
* Backend
* Seguridad
* Datos
* GDPR/Privacidad
* Infraestructura

### Criterios de Aceptación

* El sistema debe permitir almacenar perfiles completos de candidatos incluyendo información personal, de contacto, experiencia, educación, habilidades y documentación adicional.
* La base de datos debe admitir la subida y visualización de múltiples formatos de documentos (PDF, DOC, DOCX, JPG) con un tamaño máximo de 10MB por archivo.
* Debe implementarse un sistema de búsqueda que permita filtrar candidatos por al menos 10 criterios diferentes, incluyendo cargo, experiencia, ubicación, habilidades, disponibilidad y fuente de reclutamiento.
* El sistema debe mantener un historial completo de cada candidato, incluyendo todas las posiciones a las que ha aplicado, estados y evaluaciones previas.
* La estructura de datos debe permitir la categorización de candidatos mediante etiquetas personalizables y la creación de listas de candidatos para diferentes propósitos.
* La implementación debe cumplir con las regulaciones de protección de datos (GDPR, CCPA, etc.) incluyendo retención de datos limitada, consentimiento explícito y derechos de acceso/eliminación.
* El sistema debe ofrecer permisos granulares para acceder a diferentes tipos de información según el rol del usuario.
* La base de datos debe soportar la importación masiva de perfiles mediante archivos CSV y la exportación de datos para análisis externo.
* La arquitectura debe ser escalable para manejar al menos 100,000 perfiles de candidatos con un tiempo de respuesta máximo de 3 segundos para búsquedas complejas.
* El sistema debe registrar todas las modificaciones realizadas a los datos de los candidatos, manteniendo un log auditable.
 
### Notas Adicionales

* Esta historia representa la funcionalidad más fundamental del sistema y servirá como base para la mayoría de las otras características.
* Se deberá considerar la implementación de técnicas de cifrado para datos sensibles.
* Será necesario diseñar un esquema de datos flexible que permita futuras extensiones sin necesidad de modificaciones estructurales importantes.
* El rendimiento es crítico ya que esta base de datos será consultada constantemente.
* Considerar la posibilidad de implementar capacidades de detección de perfiles duplicados.
* La estrategia de backup y recuperación debe ser robusta, con copias de seguridad programadas y capacidad de recuperación puntual.
* Evaluar la necesidad de un servicio de CDN para la entrega eficiente de documentos adjuntos.
* La base de datos debe estar diseñada para soportar operaciones internacionales con consideraciones para múltiples idiomas y regiones.

### Historias de Usuario Relacionadas

- "Filtrado automático de candidaturas" (dependencia directa)
- "Búsquedas avanzadas en banco de talentos" (dependencia directa)
- "Cumplimiento de regulaciones de protección de datos" (dependencia parcial)
- "Visualización de estados de candidatos" (dependencia parcial)
- "Evaluación colaborativa de candidatos" (dependencia indirecta)

### Tareas

1. Realizar análisis de requisitos detallado con stakeholders para definir todos los campos necesarios.
2. Diseñar modelo de datos considerando escalabilidad y relaciones entre entidades.
3. Implementar esquema de base de datos con índices optimizados para rendimiento.
4. Desarrollar APIs RESTful para CRUD de perfiles de candidatos.
5. Implementar sistema de búsqueda con indexación eficiente.
6. Desarrollar funcionalidades de importación/exportación de datos.
7. Implementar mecanismos de seguridad (cifrado, control de acceso, auditoría).
8. Desarrollar sistema de almacenamiento de documentos adjuntos con verificación de tipos y antivirus.
9. Crear pruebas unitarias y de integración.
10. Diseñar e implementar la estrategia de respaldo y recuperación.
11. Documentar la arquitectura de datos y APIs.
12. Realizar pruebas de carga para verificar el rendimiento con grandes volúmenes de datos.
13. Implementar políticas de retención y eliminación automatizada de datos según normativas.
14. Desarrollar dashboard de administración para monitoreo y mantenimiento.

### Enlaces

* [GDPR Compliance Checklist](https://gdpr.eu/checklist/)
* [MongoDB vs PostgreSQL for Candidate Management](https://www.mongodb.com/compare/mongodb-postgresql)
* [AWS Best Practices for Document Storage](https://aws.amazon.com/solutions/implementations/document-management-on-aws/)
* [Elasticsearch for Recruitment Data](https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html)
* [OWASP Security Practices for Personal Data](https://owasp.org/www-project-top-ten/)
* [Data Modeling for HR Systems](https://www.oreilly.com/library/view/data-model-patterns/9780120887989/)


## Historia de Usuario: Publicación de Ofertas en Portal Corporativo

Título: Publicación de Ofertas en Portal Corporativo

Como reclutador,
quiero crear y publicar ofertas de empleo en el portal corporativo del ATS,
para gestionar de forma centralizada las vacantes y hacerlas visibles a los candidatos potenciales.

### Descripción

Esta funcionalidad permitirá a los reclutadores crear ofertas de empleo completas utilizando un editor estructurado y publicarlas en el portal de empleo corporativo integrado en el ATS. La creación de ofertas incluirá campos estándar y personalizables, opciones para establecer fechas de publicación/caducidad, y un proceso de revisión/aprobación cuando sea necesario. Una vez publicadas, las ofertas serán visibles para los candidatos en el portal público, donde podrán ver los detalles y aplicar directamente.

### Prioridad
Alta

### Story points

8

### Estimación

| Metodología | Valoración | Significado |
| --- | --- | --- |
| Fibonacci | 8   | Complejidad media-alta con elementos conocidos |
| Planning Poker | 8   | Consenso del equipo sobre esfuerzo significativo pero manejable |
| Talla de camiseta | L   | Esfuerzo considerable, equivalente a 1-2 semanas de trabajo |

### Asignado a

* Frontend (principal)
* Backend
* Diseñador UX/UI

### Etiquetas

* Core
* Frontend
* Backend
* Publicación
* UX/UI
* Workflow

### Criterios de Aceptación

* El sistema debe proporcionar un formulario estructurado con todos los campos relevantes para crear una oferta laboral completa (título, departamento, ubicación, tipo de contrato, descripción, requisitos, responsabilidades, beneficios, etc.).
* Los reclutadores deben poder guardar borradores de ofertas para completarlas posteriormente.
* El sistema debe permitir la vista previa de cómo se verá la oferta en el portal antes de publicarla.
* Los usuarios con permisos adecuados deben poder establecer fechas de publicación y caducidad para las ofertas.
* El sistema debe implementar un flujo de aprobación configurable para organizaciones que requieran validación antes de la publicación.
* Las ofertas publicadas deben ser inmediatamente visibles en el portal público de empleo con un formato optimizado para la lectura.
* El sistema debe incluir funcionalidad para cerrar, pausar, renovar o editar ofertas ya publicadas.
* Los reclutadores deben poder duplicar ofertas existentes para crear nuevas similares, optimizando tiempo.
* El sistema debe proporcionar estadísticas básicas sobre cada oferta (visualizaciones, aplicaciones recibidas, tasa de conversión).
* Las ofertas deben ser categorizadas automáticamente por departamento, ubicación y área funcional para facilitar la navegación en el portal.
* El sistema debe soportar la publicación en múltiples idiomas para organizaciones internacionales.
* Las ofertas deben ser optimizadas para SEO con metadatos y estructura adecuada.

### Notas Adicionales

* El diseño del editor debe equilibrar facilidad de uso con flexibilidad para crear ofertas atractivas.
* La interfaz de creación debe ser intuitiva y minimizar la curva de aprendizaje para nuevos reclutadores.
* Es importante considerar la velocidad de carga del portal público para mejorar la experiencia del candidato.
* El sistema debe implementar manejo de versiones para las ofertas editadas, manteniendo histórico de cambios.
* Considerar la implementación de plantillas predefinidas para agilizar la creación de ofertas estándar.
* Evaluar la posibilidad de A/B testing para diferentes formatos o textos de ofertas.
* La arquitectura debe permitir la fácil extensión para la integración con canales externos en el futuro (Historia 1B).
* Se deben considerar prácticas de accesibilidad (WCAG 2.1) para el portal público.
* El rendimiento del portal debe optimizarse para dispositivos móviles, con un enfoque mobile-first.

### Historias de Usuario Relacionadas

* "Base de datos centralizada de candidatos" (dependencia indirecta)
* "Integración con Canales Externos de Empleo" (historia sucesora)
* "Personalización con imagen corporativa" (complementaria)
* "Filtrado automático de candidaturas" (dependencia indirecta)
* "Visualización de estados de candidatos" (dependencia parcial)

### Tareas

1. Diseñar la arquitectura del sistema de publicación y almacenamiento de ofertas.
2. Crear wireframes y mockups de la interfaz de creación de ofertas.
3. Diseñar la UI/UX del portal público de empleo, incluyendo vistas de listado y detalle.
4. Desarrollar el modelo de datos para almacenar ofertas y sus estados.
5. Implementar la API RESTful para gestión de ofertas (CRUD).
6. Desarrollar el editor de ofertas con todos los campos requeridos.
7. Implementar el sistema de guardado de borradores y versionado.
8. Desarrollar la funcionalidad de vista previa.
9. Implementar el flujo de aprobación configurable.
10. Desarrollar el portal público con funcionalidades de búsqueda y filtrado.
11. Implementar el sistema de fechas de publicación/caducidad.
12. Crear el dashboard de estadísticas básicas por oferta.
13. Optimizar la interfaz para dispositivos móviles.
14. Implementar pruebas de usabilidad con usuarios reales.
15. Desarrollar pruebas unitarias y de integración.
16. Documentar la API y las funcionalidades para usuarios finales.

### Enlaces

* [Nielsen Norman Group: Job Posting UX Best Practices](https://www.nngroup.com/articles/job-ad-design/)
* [Google for Jobs Schema Guidelines](https://developers.google.com/search/docs/appearance/structured-data/job-posting)
* [Material Design Components for Form Design](https://material.io/components/text-fields/overview)
* [Web Content Accessibility Guidelines (WCAG 2.1)](https://www.w3.org/TR/WCAG21/)
* [React Final Form for Complex Forms](https://final-form.org/react)
* [Best Practices for SEO in Job Listings](https://www.linkedin.com/business/talent/blog/talent-acquisition/seo-best-practices-for-job-descriptions)
* [JWT Authentication for Multi-step Form Processes](https://jwt.io/introduction/)
* [Responsive Design Patterns for Form Implementation](https://bradfrost.com/blog/post/responsive-web-design-patterns/)