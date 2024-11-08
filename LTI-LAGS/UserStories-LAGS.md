# User Stories

#### 1. **User Story: Asignación Automática de Candidatos a Vacantes**

**Descripción**: Como **reclutador**, quiero que el sistema realice una asignación automática de los candidatos a vacantes relevantes, basada en sus habilidades y experiencia, para optimizar el proceso de preselección.

**Criterios de Aceptación**:
- **Dado** que el candidato ha completado su perfil, **cuando** el sistema detecta una coincidencia con una vacante, **entonces** asigna automáticamente al candidato a esa vacante.
- **Dado** que un candidato es asignado automáticamente a una vacante, **cuando** el reclutador revisa la lista de candidatos asignados, **entonces** puede ver al candidato en la vacante correspondiente.

**Notas Adicionales**:
- La asignación debe realizarse en tiempo real y permitir personalización en los criterios de búsqueda.

**Tareas**:
- Integrar el sistema de emparejamiento de IA para candidatos.
- Configurar notificaciones para alertas de asignación automática.
- Realizar pruebas de integración y validar la funcionalidad de asignación automática.

---

#### 2. **User Story: Panel de Colaboración en Tiempo Real para Reclutadores y Managers**

**Descripción**: Como **reclutador**, quiero un panel de colaboración en tiempo real para intercambiar comentarios con los managers de contratación, facilitando una toma de decisiones rápida y organizada.

**Criterios de Aceptación**:
- **Dado** que el reclutador ha seleccionado una vacante, **cuando** agrega un comentario o etiqueta al manager, **entonces** el manager recibe una notificación en tiempo real.
- **Dado** que un manager revisa una vacante, **cuando** ve los comentarios en el panel, **entonces** puede responder o realizar aprobaciones directamente en el sistema.

**Notas Adicionales**:
- Incluir opciones de filtrado para comentarios específicos de cada candidato.

**Tareas**:
- Desarrollar la interfaz de colaboración en tiempo real.
- Integrar notificaciones y alertas para el equipo.
- Probar la funcionalidad de comentarios y etiquetado en tiempo real.

---

#### 3. **User Story: Portal Personalizado para Seguimiento del Progreso del Candidato**

**Descripción**: Como **candidato**, quiero un portal personalizado donde pueda ver mi progreso en el proceso de selección, para mantenerme informado y comprometido.

**Criterios de Aceptación**:
- **Dado** que el candidato inicia sesión en el portal, **cuando** revisa su perfil, **entonces** puede ver el estado actual de cada etapa del proceso de selección.
- **Dado** que el reclutador actualiza el estado del candidato, **cuando** el candidato accede al portal, **entonces** ve el cambio reflejado en tiempo real.

**Notas Adicionales**:
- Incluir notificaciones automáticas de cambios en el estado.

**Tareas**:
- Diseñar y desarrollar el portal de candidatos.
- Configurar notificaciones automáticas para cambios de estado.
- Pruebas de experiencia de usuario para asegurar la fluidez y claridad del portal.

---

#### 4. **User Story: Automatización de Programación de Entrevistas con IA**

**Descripción**: Como **reclutador**, quiero que el sistema programe automáticamente entrevistas con los candidatos, utilizando IA para encontrar horarios convenientes, para ahorrar tiempo y evitar conflictos.

**Criterios de Aceptación**:
- **Dado** que el candidato ha sido seleccionado para entrevista, **cuando** el sistema busca en los calendarios, **entonces** sugiere automáticamente horarios disponibles para ambas partes.
- **Dado** que el candidato y el reclutador han confirmado un horario, **cuando** se programa la entrevista, **entonces** ambos reciben una confirmación con los detalles del encuentro.

**Notas Adicionales**:
- La funcionalidad debe integrarse con calendarios externos como Google Calendar y Outlook.

**Tareas**:
- Implementar la funcionalidad de IA para sugerencia de horarios.
- Integrar API de Google Calendar y Outlook para disponibilidad de horarios.
- Realizar pruebas de funcionalidad para asegurar la precisión en la programación.

---

#### 5. **User Story: Evaluación Predictiva de Talento con Algoritmos de IA**

**Descripción**: Como **manager de contratación**, quiero que el sistema realice evaluaciones predictivas del talento de los candidatos, basándose en pruebas de personalidad y habilidades, para seleccionar a los candidatos más adecuados.

**Criterios de Aceptación**:
- **Dado** que un candidato ha completado las evaluaciones, **cuando** el sistema genera un perfil predictivo, **entonces** el manager puede ver una evaluación sobre su adecuación cultural y técnica.
- **Dado** que se revisan varios perfiles, **cuando** el manager compara candidatos, **entonces** puede ver las puntuaciones predictivas en una misma vista para facilitar la comparación.

**Notas Adicionales**:
- El sistema debe permitir personalizar los parámetros de evaluación según el puesto.

**Tareas**:
- Desarrollar el sistema de evaluación predictiva utilizando algoritmos de IA.
- Integrar pruebas de personalidad y técnicas en el sistema.
- Realizar pruebas de precisión y validez en las evaluaciones.

---

#### 6. **User Story: Notificaciones Personalizadas de Progreso para Candidatos**

**Descripción**: Como **candidato**, quiero recibir notificaciones personalizadas sobre el progreso de mi solicitud, para estar informado en tiempo real sobre cada etapa del proceso.

**Criterios de Aceptación**:
- **Dado** que el estado de un candidato cambia, **cuando** el sistema detecta el cambio, **entonces** envía automáticamente una notificación al candidato.
- **Dado** que el candidato ha configurado sus preferencias de notificación, **cuando** se realiza un cambio en su perfil, **entonces** recibe una notificación según sus preferencias.

**Notas Adicionales**:
- Incluir opciones para configurar la frecuencia y tipo de notificaciones.

**Tareas**:
- Configurar notificaciones personalizadas y opciones de preferencia.
- Integrar sistema de notificaciones en tiempo real.
- Realizar pruebas de funcionalidad y UX para asegurar la claridad de las notificaciones.
  
---
<br><br>

# Backlog de producto 

## **Metodología usada:** RICE

### Detalles de los Factores de la Metodología RICE

1. **Alcance (Reach)**: Número de usuarios o candidatos que se verán beneficiados o que utilizarán la funcionalidad en un tiempo determinado (por ejemplo, mensual).
2. **Impacto (Impact)**: La influencia o cambio positivo que se espera que la funcionalidad tenga en la experiencia del usuario o en la eficiencia del proceso. Se mide en una escala de 1 a 5, donde 5 es un impacto muy alto.
3. **Confianza (Confidence)**: El grado de seguridad que tiene el equipo en la efectividad de la funcionalidad. Se mide en porcentaje (0-100%), considerando la claridad de los requerimientos y la viabilidad.
4. **Esfuerzo (Effort)**: Estimación del tiempo o puntos necesarios para completar la tarea, considerando la complejidad técnica y los recursos. El esfuerzo se mide en semanas.

---

### Backlog de Producto Priorizado (Tabla RICE)

| **User Story**                                    | **Descripción**                                                                                                   | **Reach** | **Impact** | **Confidence** | **Effort** | **Puntaje RICE** | **Prioridad** |
|---------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|-----------|------------|----------------|------------|------------------|---------------|
| **Portal Personalizado para Seguimiento del Progreso del Candidato** | Proporcionar a los candidatos un portal donde pueden ver el progreso de su solicitud y recibir actualizaciones.      | 1000      | 3          | 90%            | 4          | 675              | Alta          |
| **Asignación Automática de Candidatos a Vacantes**| Permitir que el sistema asigne automáticamente candidatos a vacantes relevantes en base a sus habilidades.        | 800       | 4          | 80%            | 4          | 640              | Alta          |
| **Notificaciones Personalizadas de Progreso para Candidatos**        | Enviar notificaciones personalizadas a los candidatos para informarles sobre el estado de su solicitud.             | 1000      | 2          | 90%            | 3          | 600              | Alta          |
| **Evaluación Predictiva de Talento con Algoritmos de IA**           | Generar evaluaciones predictivas sobre el talento de los candidatos para ayudar a los managers en la selección.     | 600       | 4          | 80%            | 5          | 384              | Media         |
| **Automatización de Programación de Entrevistas con IA**            | Programar automáticamente entrevistas basándose en la disponibilidad de candidatos y reclutadores mediante IA.      | 600       | 3          | 80%            | 4          | 360              | Media         |
| **Panel de Colaboración en Tiempo Real para Reclutadores y Managers**| Proveer un panel colaborativo donde reclutadores y managers puedan intercambiar comentarios en tiempo real.         | 700       | 3          | 85%            | 5          | 357              | Baja          |

---

#### Detalle de cada User Story en el Backlog

---

##### 1. **User Story: Portal Personalizado para Seguimiento del Progreso del Candidato**

- **Descripción**: Como candidato, quiero un portal personalizado donde pueda ver mi progreso en el proceso de selección, para mantenerme informado y comprometido.
- **Criterios de Aceptación**:
  - El candidato puede ver el estado actual de cada etapa de selección al acceder al portal.
  - Los cambios de estado en tiempo real se reflejan inmediatamente en el portal.
- **Tareas**:
  - Diseñar y desarrollar el portal de candidatos.
  - Configurar notificaciones automáticas de cambio de estado.
  - Realizar pruebas de experiencia de usuario.
- **Prioridad**: Alta (Puntaje RICE: 675)

---

##### 2. **User Story: Asignación Automática de Candidatos a Vacantes**

- **Descripción**: Como reclutador, quiero que el sistema realice una asignación automática de los candidatos a vacantes relevantes, basada en sus habilidades y experiencia.
- **Criterios de Aceptación**:
  - Los candidatos con perfiles que coincidan con una vacante son asignados automáticamente.
  - Los reclutadores pueden ver las asignaciones automáticas en la lista de candidatos.
- **Tareas**:
  - Integrar el sistema de emparejamiento de IA.
  - Configurar notificaciones de asignación automática.
  - Validar funcionalidad de asignación.
- **Prioridad**: Alta (Puntaje RICE: 640)

---

##### 3. **User Story: Notificaciones Personalizadas de Progreso para Candidatos**

- **Descripción**: Como candidato, quiero recibir notificaciones personalizadas sobre el progreso de mi solicitud en tiempo real.
- **Criterios de Aceptación**:
  - El candidato recibe notificaciones automáticas al cambiar el estado de su solicitud.
  - El candidato puede personalizar la frecuencia de sus notificaciones.
- **Tareas**:
  - Configurar notificaciones personalizadas y opciones de preferencia.
  - Integrar el sistema de notificaciones en tiempo real.
  - Pruebas de funcionalidad y UX.
- **Prioridad**: Alta (Puntaje RICE: 600)

---

##### 4. **User Story: Evaluación Predictiva de Talento con Algoritmos de IA**

- **Descripción**: Como manager de contratación, quiero que el sistema realice evaluaciones predictivas del talento de los candidatos para seleccionar a los más adecuados.
- **Criterios de Aceptación**:
  - El manager puede ver una evaluación predictiva del ajuste cultural y técnico del candidato.
  - Las evaluaciones se pueden comparar en una misma vista.
- **Tareas**:
  - Desarrollar el sistema de evaluación predictiva.
  - Integrar pruebas de personalidad y técnicas.
  - Pruebas de precisión y validez.
- **Prioridad**: Media (Puntaje RICE: 384)

---

##### 5. **User Story: Automatización de Programación de Entrevistas con IA**

- **Descripción**: Como reclutador, quiero que el sistema programe automáticamente entrevistas con los candidatos, utilizando IA para encontrar horarios convenientes.
- **Criterios de Aceptación**:
  - La IA sugiere horarios disponibles de entrevistas basándose en calendarios de los candidatos y reclutadores.
  - Las confirmaciones de entrevista son automáticas y se envían a ambas partes.
- **Tareas**:
  - Implementar la funcionalidad de IA para programación.
  - Integrar API de Google Calendar y Outlook.
  - Realizar pruebas de funcionalidad.
- **Prioridad**: Media (Puntaje RICE: 360)

---

##### 6. **User Story: Panel de Colaboración en Tiempo Real para Reclutadores y Managers**

- **Descripción**: Como reclutador, quiero un panel de colaboración en tiempo real para intercambiar comentarios con los managers de contratación.
- **Criterios de Aceptación**:
  - Los managers y reclutadores pueden ver comentarios en tiempo real y responder.
  - Notificaciones automáticas de nuevos comentarios y aprobaciones.
- **Tareas**:
  - Desarrollar la interfaz de colaboración.
  - Integrar notificaciones y alertas en tiempo real.
  - Probar comentarios y etiquetado.
- **Prioridad**: Baja (Puntaje RICE: 357)

--- 
<br><br>

# Tickets de trabajo

**1. User Story: Asignación Automática de Candidatos a Vacantes**  

---

### Etapa 1: Diseño de la Interfaz del Portal de Candidatos

### 1. **Título**: Diseño de la interfaz del portal de candidatos

- **Descripción**:
  - **Propósito**: Crear un diseño de interfaz de usuario intuitiva y atractiva para que los candidatos puedan revisar su progreso en el proceso de selección.
  - **Detalles Específicos**: Diseñar una interfaz responsiva y amigable para dispositivos móviles y de escritorio. Debe mostrar el estado de cada etapa del proceso de selección y permitir notificaciones de cambios en tiempo real.
  
- **Criterios de Aceptación**:
  - El diseño debe cumplir con las pautas de accesibilidad y ser fácil de navegar.
  - La interfaz debe ser responsiva, adaptándose a diferentes tamaños de pantalla.
  - Debe incluir elementos de interfaz básicos como barra de progreso, visualización de estados y notificaciones de cambios.

- **Prioridad**: Alta
- **Asignación**: Equipo de UI/UX Design
- **Etiquetas**: UI, Diseño, Sprint 1
- **Comentarios y Notas**: Revisión del diseño con el equipo de desarrollo antes de pasar a la etapa de implementación.
- **Enlaces o Referencias**: Enlace al prototipo inicial de la interfaz en Figma.
- **Historial de Cambios**: Ninguno.

---

### 2. **Título**: Implementación de la interfaz de usuario del portal de candidatos

- **Descripción**:
  - **Propósito**: Implementar el diseño del portal de candidatos en el frontend para mostrar la información de progreso.
  - **Detalles Específicos**: Utilizar tecnologías como React para el frontend. La interfaz debe consumir datos desde la API para reflejar el estado de cada etapa del proceso de selección en tiempo real.

- **Criterios de Aceptación**:
  - La interfaz de usuario debe visualizar correctamente el progreso de cada etapa.
  - El portal debe ser responsivo y reflejar cualquier cambio de estado de forma dinámica.

- **Prioridad**: Alta
- **Asignación**: Equipo de Frontend
- **Etiquetas**: UI, Frontend, Sprint 1
- **Comentarios y Notas**: Asegurarse de que el diseño esté alineado con las especificaciones de accesibilidad y usabilidad.
- **Enlaces o Referencias**: Prototipo de interfaz en Figma, API para el estado de candidatos.
- **Historial de Cambios**: Ninguno.

---

### Etapa 2: Backend para la Gestión de Estado de Proceso del Candidato

### 3. **Título**: Creación de API para estado de proceso de selección de candidatos

- **Descripción**:
  - **Propósito**: Proporcionar una API que permita obtener el estado de cada candidato en su proceso de selección, actualizándolo en tiempo real en el portal.
  - **Detalles Específicos**: Crear una API RESTful que entregue el estado actual del candidato y que permita actualizarlo cuando se modifiquen sus etapas de proceso.

- **Criterios de Aceptación**:
  - La API debe devolver el estado actual del candidato y permitir actualizaciones en tiempo real.
  - Debe contar con una documentación clara para el uso de endpoints.

- **Prioridad**: Alta
- **Asignación**: Equipo de Backend
- **Etiquetas**: Backend, API, Sprint 1
- **Comentarios y Notas**: Coordinar con el equipo de frontend para asegurar la correcta integración.
- **Enlaces o Referencias**: Documentación de la API, User Story de portal de candidatos.
- **Historial de Cambios**: Ninguno.

---

### 4. **Título**: Configuración de base de datos para el seguimiento de etapas del proceso de selección

- **Descripción**:
  - **Propósito**: Configurar la base de datos para almacenar el estado de cada etapa del proceso de selección de cada candidato.
  - **Detalles Específicos**: Definir un modelo de datos en la base de datos que permita almacenar y actualizar el estado de los candidatos de manera escalable.

- **Criterios de Aceptación**:
  - La base de datos debe permitir la creación, actualización y consulta de cada etapa del proceso de selección de un candidato.
  - Debe soportar la actualización en tiempo real para integrarse con la API.

- **Prioridad**: Alta
- **Asignación**: Equipo de Backend
- **Etiquetas**: Base de datos, Backend, Sprint 1
- **Comentarios y Notas**: Asegurarse de la escalabilidad y rendimiento de la base de datos para soportar un alto volumen de solicitudes.
- **Enlaces o Referencias**: Especificación del modelo de datos, Documento de la User Story.
- **Historial de Cambios**: Ninguno.

---

### Etapa 3: Implementación de Notificaciones Automáticas en Tiempo Real

### 5. **Título**: Configuración de sistema de notificaciones en tiempo real

- **Descripción**:
  - **Propósito**: Configurar el sistema de notificaciones en tiempo real para que los candidatos reciban actualizaciones automáticas de cambios en su estado.
  - **Detalles Específicos**: Utilizar WebSockets o un sistema de mensajería (Firebase, AWS SNS) para enviar notificaciones en tiempo real cuando el estado de un candidato se actualice.

- **Criterios de Aceptación**:
  - El sistema debe enviar notificaciones automáticamente al candidato cada vez que se actualice su estado.
  - Las notificaciones deben funcionar de forma óptima en tiempo real sin demoras perceptibles.

- **Prioridad**: Media
- **Asignación**: Equipo de Backend y DevOps
- **Etiquetas**: Backend, Integración, Notificaciones, Sprint 2
- **Comentarios y Notas**: Coordinar con frontend para visualizar las notificaciones en el portal de candidatos.
- **Enlaces o Referencias**: Documentación de Firebase y AWS SNS.
- **Historial de Cambios**: Ninguno.

---

### 6. **Título**: Implementación de notificaciones en la interfaz del portal de candidatos

- **Descripción**:
  - **Propósito**: Implementar en la interfaz de usuario las notificaciones en tiempo real cuando el estado de los candidatos cambia.
  - **Detalles Específicos**: Mostrar notificaciones no intrusivas en el portal, utilizando las notificaciones configuradas en el backend.

- **Criterios de Aceptación**:
  - El candidato debe recibir una notificación visual en el portal cuando se actualice su estado.
  - La notificación debe ser visible y fácil de entender, sin interrumpir la navegación en el portal.

- **Prioridad**: Media
- **Asignación**: Equipo de Frontend
- **Etiquetas**: UI, Notificaciones, Frontend, Sprint 2
- **Comentarios y Notas**: Pruebas de usabilidad para asegurar que las notificaciones sean claras y efectivas.
- **Enlaces o Referencias**: Documentación de WebSockets, Firebase y AWS SNS.
- **Historial de Cambios**: Ninguno.

---

### Etapa 4: Pruebas de Funcionalidad e Integración

### 7. **Título**: Pruebas de integración entre frontend y backend del portal de candidatos

- **Descripción**:
  - **Propósito**: Asegurar que todos los componentes del portal (frontend, backend y notificaciones) funcionen juntos sin problemas.
  - **Detalles Específicos**: Realizar pruebas de integración para verificar que los datos se actualicen correctamente y que las notificaciones se envíen y muestren en tiempo real.

- **Criterios de Aceptación**:
  - La integración debe funcionar sin errores, con datos actualizados y notificaciones en tiempo real.
  - Todas las pruebas deben pasar y los errores identificados deben resolverse antes de implementar en producción.

- **Prioridad**: Alta
- **Asignación**: Equipo de QA y Soporte
- **Etiquetas**: QA, Integración, Sprint 3
- **Comentarios y Notas**: Registrar y solucionar cualquier error encontrado en un documento de control de calidad.
- **Enlaces o Referencias**: Documentación de QA, Pruebas automatizadas.
- **Historial de Cambios**: Ninguno.

--- 
<br><br>

### 8. **Título**: Pruebas de experiencia de usuario y accesibilidad en el portal de candidatos

- **Descripción**:
  - **Propósito**: Asegurar que el portal de candidatos sea accesible, intuitivo y fácil de usar.
  - **Detalles Específicos**: Realizar pruebas de usabilidad y accesibilidad para garantizar que el portal cumpla con los estándares WCAG y sea intuitivo para los candidatos.

- **Criterios de Aceptación**:
  - El portal debe ser completamente accesible y fácil de usar, cumpliendo con las pautas WCAG.
  - Los candidatos deben poder navegar intuitivamente y ver el progreso sin problemas.

- **Prioridad**: Media
- **Asignación**: Equipo de QA y UX
- **Etiquetas**: QA, UX, Accesibilidad, Sprint 3
- **Comentarios y Notas**: Documentar los resultados y solucionar cualquier problema antes de la implementación final.
- **Enlaces o Referencias**: Especificaciones WCAG.
- **Historial de Cambios**: Ninguno.

---


# Estimación tikets de trabajo


Aquí tienes una tabla en formato Markdown con las estimaciones iniciales en horas para cada ticket de trabajo. Estas estimaciones están basadas en el consenso del equipo de desarrollo utilizando la metodología **Planning Poker**.

| **Ticket**                                           | **Estimación (Horas)** | **Justificación**                                                                                                                                                       |
|------------------------------------------------------|-------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1. Diseño de la Interfaz del Portal de Candidatos    | 12 horas               | Considera el tiempo para desarrollar un diseño responsivo e intuitivo, asegurando la coherencia con las pautas de diseño de la empresa.                                  |
| 2. Implementación de la Interfaz en Frontend         | 20 horas               | Incluye el desarrollo de la interfaz funcional en frontend y las pruebas de visualización en dispositivos móviles y de escritorio.                                      |
| 3. Configuración de Notificaciones en Tiempo Real    | 16 horas               | Se estima en función de la integración del sistema de notificaciones en tiempo real, incluyendo pruebas y ajustes de personalización de alertas.                         |
| 4. Configuración de Preferencias de Notificación en la Interfaz | 10 horas | Considera el esfuerzo de añadir opciones de configuración en la interfaz y asegurar la persistencia en el backend.                                                      |
| 5. Integración de Actualización en Tiempo Real con Backend | 18 horas | Evaluación de la complejidad de la comunicación en tiempo real entre frontend y backend, incluyendo pruebas de estabilidad.                                              |
| 6. Persistencia y Almacenamiento de Preferencias de Notificación | 12 horas | Incluye la configuración de bases de datos para almacenar las preferencias de notificación y asegurar la seguridad en la manipulación de datos de usuarios.              |
| 7. Pruebas de Funcionalidad del Portal               | 15 horas               | Estimación basada en pruebas exhaustivas de cada funcionalidad del portal, especialmente la actualización en tiempo real y notificaciones.                               |
| 8. Pruebas de Rendimiento y Escalabilidad           | 14 horas               | Considera pruebas de rendimiento bajo cargas altas y ajustes para garantizar la escalabilidad del portal.                                                               |



### Resumen de Justificaciones Clave:

1. **Diseño de la Interfaz del Portal**: Requiere tiempo para un diseño claro, visualmente atractivo y alineado con los lineamientos de la empresa.
2. **Implementación de la Interfaz en Frontend**: La traducción del diseño a frontend incluye la funcionalidad y pruebas de responsividad.
3. **Notificaciones en Tiempo Real**: Se estima una alta complejidad debido a la personalización y la necesidad de sincronización en tiempo real.
4. **Preferencias de Notificación en la Interfaz**: Requiere integración con backend y opciones de configuración accesibles para el usuario.
5. **Actualización en Tiempo Real con Backend**: La complejidad de la comunicación en tiempo real y pruebas de estabilidad afectan la estimación.
6. **Persistencia de Preferencias**: Asegurar el almacenamiento seguro de datos y la capacidad de modificación en tiempo real.
7. **Pruebas de Funcionalidad**: Incluye pruebas de cada función clave, priorizando la actualización en tiempo real y la precisión de notificaciones.
8. **Pruebas de Rendimiento**: Enfocadas en garantizar que el portal sea escalable y funcione sin problemas bajo alta carga de usuarios.

Esta tabla proporciona una referencia clara de las estimaciones acordadas, alineadas con las prioridades y requisitos del proyecto.