# Historia de Usuario 1: Creación de ofertas laborales

## Título de la Historia de Usuario
**Creación de ofertas laborales**

## Descripción
Como **Reclutador**, quiero crear una nueva oferta laboral con todos los detalles necesarios, para que pueda iniciar el proceso de reclutamiento para una posición requerida.

## Criterios de Aceptación
- Debe existir un formulario con campos para: título del puesto, descripción, requisitos, ubicación, tipo de contrato y rango salarial.
- El sistema debe validar que todos los campos obligatorios estén completos.
- Al guardar, la oferta debe pasar al estado "Pendiente de aprobación".
- Debe generarse una vista previa de cómo se verá la oferta publicada.

## Notas Adicionales
- Considerar la inclusión de campos personalizables por departamento.
- La interfaz debe ser intuitiva y permitir guardar borradores.

## Historias de Usuario Relacionadas
- Edición de ofertas laborales
- Aprobación de ofertas laborales

---

# Historia de Usuario 2: Aprobación de ofertas laborales

## Título de la Historia de Usuario
**Aprobación de ofertas laborales**

## Descripción
Como **Gerente de Contratación**, quiero revisar y aprobar las ofertas laborales creadas por los reclutadores, para que se publiquen contenidos de calidad que representen adecuadamente a la empresa.

## Criterios de Aceptación
- Debe existir una bandeja de ofertas pendientes de aprobación.
- El gerente debe poder ver todos los detalles de la oferta.
- Debe poder aprobar, rechazar o solicitar cambios a la oferta.
- Al aprobar, la oferta debe pasar automáticamente al proceso de publicación.
- Al rechazar o solicitar cambios, debe poder incluir comentarios.

## Notas Adicionales
- Implementar notificaciones por email cuando una oferta requiere aprobación.
- Considerar un flujo de aprobación configurable por departamento o tipo de posición.

## Historias de Usuario Relacionadas
- Creación de ofertas laborales
- Publicación de ofertas laborales

---

# Historia de Usuario 3: Publicación multi-canal de ofertas

## Título de la Historia de Usuario
**Publicación multi-canal de ofertas**

## Descripción
Como **Reclutador**, quiero publicar ofertas aprobadas en múltiples canales simultáneamente, para que pueda maximizar el alcance y atraer más candidatos calificados.

## Criterios de Aceptación
- Debe permitir seleccionar desde una lista los canales donde publicar (portal de carreras, bolsas de trabajo, redes sociales).
- Debe adaptar automáticamente el formato de la oferta según el canal.
- Debe mostrar confirmación de publicación exitosa o errores si ocurren.
- Debe permitir programar la fecha y hora de publicación.

## Notas Adicionales
- Integrar con APIs de las principales bolsas de trabajo.
- Permitir personalizar el mensaje para cada canal.

## Historias de Usuario Relacionadas
- Aprobación de ofertas laborales
- Estadísticas de ofertas publicadas

---

# Historias de Usuario: Módulo de Pipeline de Contratación

## Historia de Usuario 4: Configuración de etapas del pipeline

## Título de la Historia de Usuario
**Configuración de etapas del pipeline**

## Descripción
Como **Gerente de Contratación**, quiero configurar las etapas del proceso de selección y sus requisitos, para que pueda adaptar el flujo según las necesidades específicas de cada departamento o posición.

## Criterios de Aceptación
- Debe permitir crear, editar y eliminar etapas del pipeline.
- Debe permitir establecer el orden de las etapas.
- Debe permitir configurar requisitos obligatorios para cada etapa.
- Debe permitir definir permisos de usuarios para mover candidatos entre etapas.

## Notas Adicionales
- Incluir plantillas predefinidas para procesos comunes.
- Permitir duplicar configuraciones existentes.

## Historias de Usuario Relacionadas
- Movimiento de candidatos en el pipeline
- Reportes de eficiencia del pipeline

---

## Historia de Usuario 5: Gestión visual de candidatos en el pipeline

## Título de la Historia de Usuario
**Gestión visual de candidatos en el pipeline**

## Descripción
Como **Reclutador**, quiero visualizar y gestionar a los candidatos en un tablero Kanban, para que pueda tener una visión clara del progreso y estado de cada candidato en el proceso.

## Criterios de Aceptación
- El tablero debe mostrar columnas correspondientes a cada etapa del pipeline.
- Cada candidato debe mostrarse como una tarjeta con información básica.
- Debe permitir arrastrar y soltar candidatos entre etapas.
- Al mover un candidato, debe solicitar la información requerida para esa etapa.
- Debe incluir filtros para buscar candidatos por nombre, posición o etapa.

## Notas Adicionales
- Implementar codificación por colores según tiempo en etapa.
- Incluir contadores de candidatos por etapa.

## Historias de Usuario Relacionadas
- Configuración de etapas del pipeline
- Programación de entrevistas

---

## Historia de Usuario 6: Automatización de comunicaciones

## Título de la Historia de Usuario
**Automatización de comunicaciones**

## Descripción
Como **Reclutador**, quiero que el sistema envíe comunicaciones automáticas a los candidatos cuando cambian de etapa, para que pueda mantener informados a los candidatos sin tareas manuales repetitivas.

## Criterios de Aceptación
- Debe permitir configurar plantillas de email para cada transición de etapa.
- Debe enviar automáticamente emails cuando un candidato cambia de etapa.
- Debe permitir personalizar variables en las plantillas (nombre del candidato, posición, etc.).
- Debe registrar un historial de comunicaciones enviadas.

## Notas Adicionales
- Considerar la inclusión de SMS además de email.
- Permitir programar recordatorios para eventos próximos.

## Historias de Usuario Relacionadas
- Gestión visual de candidatos en el pipeline
- Programación de entrevistas

---

# Historias de Usuario: Módulo de Evaluación de Candidatos

## Historia de Usuario 7: Creación de formularios de evaluación

## Título de la Historia de Usuario
**Creación de formularios de evaluación**

## Descripción
Como **Gerente de Contratación**, quiero crear formularios personalizados para evaluar candidatos, para que los entrevistadores puedan realizar evaluaciones consistentes y completas.

## Criterios de Aceptación
- Debe permitir crear formularios con diferentes tipos de preguntas (valoración numérica, selección múltiple, texto libre).
- Debe permitir agrupar preguntas por categorías (habilidades técnicas, habilidades blandas, etc.).
- Debe permitir configurar escalas de evaluación personalizadas.
- Debe permitir asignar pesos a diferentes criterios de evaluación.

## Notas Adicionales
- Incluir biblioteca de preguntas predefinidas por rol.
- Permitir duplicar y modificar formularios existentes.

## Historias de Usuario Relacionadas
- Asignación de evaluadores
- Consolidación de evaluaciones

---

## Historia de Usuario 8: Realización de evaluaciones de candidatos

## Título de la Historia de Usuario
**Realización de evaluaciones de candidatos**

## Descripción
Como **Entrevistador**, quiero completar formularios de evaluación después de entrevistar a un candidato, para que pueda documentar mis observaciones y valoraciones de manera estructurada.

## Criterios de Aceptación
- Debe mostrar el formulario asignado para la etapa y posición específica.
- Debe funcionar correctamente en dispositivos móviles.
- Debe permitir guardar borradores y completar la evaluación más tarde.
- Debe registrar automáticamente la fecha y hora de la evaluación.
- Debe permitir adjuntar archivos relevantes (ej. ejercicios realizados).

## Notas Adicionales
- Implementar recordatorios para evaluaciones pendientes.
- Considerar la posibilidad de evaluaciones sin conexión.

---

##  Plan de Implementación Sugerido
**Business Analyst: ** Basándonos en esta priorización, propongo el siguiente plan de implementación en sprints:

**Sprint 1-2 (MVP básico)**:

-Historia 1: Creación de ofertas laborales
-Historia 2: Aprobación de ofertas laborales

**Sprint 3-4:**

-Historia 5: Gestión visual de candidatos en el pipeline
-Historia 8: Realización de evaluaciones de candidatos

**Sprint 5-6**:

-Historia 3: Publicación multi-canal de ofertas
-Historia 4: Configuración de etapas del pipeline

**Sprint 7-8**:

-Historia 7: Creación de formularios de evaluación
-Historia 6: Automatización de comunicaciones

**Sprint 9-10**:

-Historia 9: Comparación y análisis de candidatos
-Refinamientos y mejoras basadas en feedback

**Metodología de Estimación**
Utilizaremos la secuencia de Fibonacci modificada para asignar los puntos de historia:

1, 2, 3, 5, 8, 13, 21, 40, 100

Donde:

-1 = Tarea muy simple
-5 = Tarea de complejidad media
-13 = Tarea compleja
-21+ = Tarea que probablemente deba dividirse

# Tickets de Trabajo - Sistema ATS (Sprint 1-2)

## Historia de Usuario 1: Creación de ofertas laborales

### TICKET ATS-001: Diseño de interfaz para creación de ofertas
**Descripción:** Diseñar la interfaz de usuario para el formulario de creación de ofertas laborales, incluyendo wireframes y maquetas de alta fidelidad.

**Tareas:**
- Diseñar wireframes de la pantalla de creación de ofertas
- Crear maquetas en alta fidelidad
- Validar diseño con stakeholders
- Documentar especificaciones de UI/UX

**Criterios de Aceptación:**
- Diseño responsivo para escritorio y móvil
- Cumple con guías de estilo de la empresa
- Incluye todos los campos requeridos
- Validado por stakeholders

**Dependencias:** Ninguna

**Asignado a:** Diseñador UI/UX

**Puntos de Historia:** 5

---

### TICKET ATS-002: Implementación del backend para gestión de ofertas
**Descripción:** Desarrollar la API REST y la capa de persistencia para la gestión de ofertas laborales.

**Tareas:**
- Crear modelo de datos para ofertas laborales
- Implementar repositorio para operaciones CRUD
- Desarrollar controladores REST para la API
- Implementar validaciones de datos
- Configurar mapeo objeto-relacional
- Escribir pruebas unitarias

**Criterios de Aceptación:**
- API implementada según especificaciones
- Todas las operaciones CRUD funcionan correctamente
- Validación adecuada de los datos de entrada
- Cobertura de pruebas unitarias > 80%
- Documentación API completa (Swagger)

**Dependencias:** Ninguna

**Asignado a:** Desarrollador Backend

**Puntos de Historia:** 8

---

### TICKET ATS-003: Implementación frontend de creación de ofertas
**Descripción:** Desarrollar el componente frontend para la creación y edición de ofertas laborales.

**Tareas:**
- Implementar formulario de creación según diseño
- Integrar con la API de backend
- Implementar validaciones del lado del cliente
- Desarrollar funcionalidad de vista previa
- Implementar guardado de borradores
- Escribir pruebas de componentes

**Criterios de Aceptación:**
- Interfaz implementada según diseños aprobados
- Validación en tiempo real de los campos
- Funcionalidad de guardar borrador operativa
- Vista previa funciona correctamente
- Pruebas de componente exitosas

**Dependencias:** ATS-001, ATS-002

**Asignado a:** Desarrollador Frontend

**Puntos de Historia:** 8

---

### TICKET ATS-004: Integración con sistema de autenticación
**Descripción:** Integrar el módulo de creación de ofertas con el sistema de autenticación para gestionar permisos.

**Tareas:**
- Configurar integración con servicio de autenticación
- Implementar control de acceso basado en roles
- Ajustar interfaces para reflejar permisos del usuario
- Probar diferentes escenarios de permisos

**Criterios de Aceptación:**
- Sólo usuarios autorizados pueden crear ofertas
- La interfaz se adapta según los permisos del usuario
- El acceso no autorizado es bloqueado correctamente
- Las acciones del usuario quedan registradas con su identidad

**Dependencias:** ATS-002, ATS-003

**Asignado a:** Desarrollador Full-stack

**Puntos de Historia:** 5

---

## Historia de Usuario 2: Aprobación de ofertas laborales

### TICKET ATS-005: Diseño de interfaz para aprobación de ofertas
**Descripción:** Diseñar la interfaz de usuario para el flujo de aprobación de ofertas laborales.

**Tareas:**
- Diseñar wireframes de bandeja de aprobaciones
- Diseñar vista detallada de oferta para revisión
- Crear maquetas en alta fidelidad
- Validar diseño con stakeholders

**Criterios de Aceptación:**
- La interfaz muestra claramente las ofertas pendientes de aprobación
- Incluye acciones para aprobar, rechazar o solicitar cambios
- Permite añadir comentarios a las decisiones
- Validado por stakeholders

**Dependencias:** ATS-001

**Asignado a:** Diseñador UI/UX

**Puntos de Historia:** 3

---

### TICKET ATS-006: Implementación del backend para flujo de aprobación
**Descripción:** Desarrollar la lógica de backend para el proceso de aprobación de ofertas laborales.

**Tareas:**
- Implementar estado de aprobación en el modelo de ofertas
- Desarrollar endpoints para gestionar el flujo de aprobación
- Implementar reglas de negocio para transiciones de estado
- Configurar registro de auditoría para aprobaciones
- Escribir pruebas unitarias

**Criterios de Aceptación:**
- API implementada según especificaciones
- Las transiciones de estado funcionan correctamente
- Se mantiene un registro completo de auditoría
- Cobertura de pruebas unitarias > 80%

**Dependencias:** ATS-002

**Asignado a:** Desarrollador Backend

**Puntos de Historia:** 5

---

### TICKET ATS-007: Implementación frontend del flujo de aprobación
**Descripción:** Desarrollar los componentes frontend para la revisión y aprobación de ofertas laborales.

**Tareas:**
- Implementar bandeja de ofertas pendientes de aprobación
- Desarrollar vista detallada de revisión
- Implementar acciones de aprobación, rechazo y solicitud de cambios
- Integrar con la API de backend
- Escribir pruebas de componentes

**Criterios de Aceptación:**
- Interfaz implementada según diseños aprobados
- Todas las acciones (aprobar, rechazar, solicitar cambios) funcionan correctamente
- Los comentarios se guardan correctamente
- Las notificaciones de estado se muestran adecuadamente
- Pruebas de componente exitosas

**Dependencias:** ATS-005, ATS-006

**Asignado a:** Desarrollador Frontend

**Puntos de Historia:** 5

---

### TICKET ATS-008: Implementación de notificaciones de aprobación
**Descripción:** Implementar sistema de notificaciones para alertar sobre ofertas pendientes de aprobación y cambios de estado.

**Tareas:**
- Integrar con servicio de email
- Configurar plantillas de notificación
- Implementar lógica de envío basada en eventos de aprobación
- Configurar preferencias de notificación por usuario
- Escribir pruebas de integración

**Criterios de Aceptación:**
- Las notificaciones se envían correctamente cuando una oferta necesita aprobación
- Se notifica al creador cuando su oferta es aprobada/rechazada
- El contenido de las notificaciones es claro y correcto
- Las preferencias de notificación funcionan correctamente

**Dependencias:** ATS-006

**Asignado a:** Desarrollador Backend

**Puntos de Historia:** 5

---

### TICKET ATS-009: Pruebas de integración del flujo completo
**Descripción:** Realizar pruebas de integración del flujo completo desde la creación hasta la aprobación de ofertas.

**Tareas:**
- Diseñar casos de prueba para flujos completos
- Implementar pruebas automatizadas end-to-end
- Realizar pruebas manuales de flujos críticos
- Documentar resultados y posibles mejoras

**Criterios de Aceptación:**
- Las pruebas cubren todos los escenarios principales y alternativos
- Todos los flujos críticos funcionan correctamente
- Se ha probado la interacción entre todos los componentes
- Se han documentado todos los defectos encontrados

**Dependencias:** ATS-004, ATS-007, ATS-008

**Asignado a:** QA Engineer

**Puntos de Historia:** 3

---

### TICKET ATS-010: Documentación de usuario
**Descripción:** Crear documentación de usuario para los módulos de creación y aprobación de ofertas.

**Tareas:**
- Redactar guías de usuario para la creación de ofertas
- Redactar guías de usuario para la aprobación de ofertas
- Crear vídeos tutoriales de los principales flujos
- Preparar materiales para capacitación

**Criterios de Aceptación:**
- La documentación cubre todas las funcionalidades implementadas
- Incluye capturas de pantalla actualizadas
- Los vídeos tutoriales son claros y muestran los flujos completos
- Revisado y aprobado por stakeholders

**Dependencias:** ATS-003, ATS-007

**Asignado a:** Technical Writer

**Puntos de Historia:** 3

# Tickets de Trabajo - Sistema ATS (Sprint 3-4)

## Historia de Usuario 5: Gestión visual de candidatos en el pipeline

### TICKET ATS-011: Diseño de interfaz Kanban para pipeline de candidatos
**Descripción:** Diseñar la interfaz de usuario del tablero Kanban para la visualización y gestión de candidatos en el pipeline.

**Tareas:**
- Diseñar wireframes del tablero Kanban
- Diseñar tarjetas de candidatos
- Crear maquetas en alta fidelidad
- Diseñar interacciones de arrastrar y soltar
- Validar diseño con stakeholders

**Criterios de Aceptación:**
- El diseño permite visualizar claramente todas las etapas del pipeline
- Las tarjetas de candidatos muestran la información esencial
- Incluye diseño de filtros y búsqueda
- La interacción de arrastrar y soltar es intuitiva
- Validado por stakeholders

**Dependencias:** Ninguna

**Asignado a:** Diseñador UI/UX

**Puntos de Historia:** 8

---

### TICKET ATS-012: Modelo de datos para pipeline de candidatos
**Descripción:** Diseñar e implementar el modelo de datos para la gestión de candidatos y etapas del pipeline.

**Tareas:**
- Diseñar el esquema de datos para candidatos
- Diseñar el esquema para etapas del pipeline
- Implementar relaciones entre ofertas, candidatos y etapas
- Configurar persistencia en DynamoDB
- Implementar índices necesarios para búsquedas eficientes
- Escribir pruebas unitarias

**Criterios de Aceptación:**
- El modelo soporta todas las operaciones necesarias
- Las relaciones entre entidades están correctamente establecidas
- Los índices permiten búsquedas eficientes
- Cobertura de pruebas unitarias > 80%

**Dependencias:** Ninguna

**Asignado a:** Desarrollador Backend

**Puntos de Historia:** 8

---

### TICKET ATS-013: API REST para gestión de pipeline
**Descripción:** Desarrollar la API REST para la gestión de candidatos en el pipeline.

**Tareas:**
- Implementar endpoints para listar candidatos por etapa
- Desarrollar funcionalidad para mover candidatos entre etapas
- Implementar filtros y búsqueda
- Desarrollar endpoints para gestión de etapas
- Documentar API con Swagger
- Escribir pruebas unitarias

**Criterios de Aceptación:**
- API implementada según especificaciones
- Soporte para todas las operaciones CRUD de candidatos
- Funcionalidad para mover candidatos entre etapas
- API documentada completamente
- Cobertura de pruebas unitarias > 80%

**Dependencias:** ATS-012

**Asignado a:** Desarrollador Backend

**Puntos de Historia:** 8

---

### TICKET ATS-014: Implementación frontend del tablero Kanban
**Descripción:** Desarrollar el componente frontend del tablero Kanban para visualización y gestión de candidatos.

**Tareas:**
- Implementar estructura del tablero Kanban
- Desarrollar tarjetas de candidatos
- Implementar funcionalidad de arrastrar y soltar
- Integrar con la API de backend
- Implementar actualización en tiempo real (opcional)
- Escribir pruebas de componente

**Criterios de Aceptación:**
- Tablero implementado según diseños aprobados
- Funcionalidad de arrastrar y soltar operativa
- Los movimientos de candidatos se guardan correctamente
- Las tarjetas muestran la información correcta
- Pruebas de componente exitosas

**Dependencias:** ATS-011, ATS-013

**Asignado a:** Desarrollador Frontend

**Puntos de Historia:** 13

---

### TICKET ATS-015: Filtros y búsqueda de candidatos
**Descripción:** Implementar funcionalidades avanzadas de filtrado y búsqueda de candidatos en el pipeline.

**Tareas:**
- Desarrollar componentes de filtros en el frontend
- Implementar lógica de búsqueda en tiempo real
- Conectar con endpoints de búsqueda y filtrado
- Implementar almacenamiento de filtros favoritos
- Escribir pruebas de componente

**Criterios de Aceptación:**
- Los filtros funcionan correctamente para todos los campos relevantes
- La búsqueda muestra resultados en tiempo real
- Los filtros favoritos se guardan correctamente
- La interfaz de filtros es intuitiva y usable
- Pruebas de componente exitosas

**Dependencias:** ATS-014

**Asignado a:** Desarrollador Frontend

**Puntos de Historia:** 5

---

### TICKET ATS-016: Recolección de información al mover candidatos
**Descripción:** Implementar la funcionalidad para solicitar información adicional cuando un candidato se mueve a determinadas etapas.

**Tareas:**
- Diseñar formularios para cada transición de etapa
- Implementar lógica para mostrar formularios según la etapa destino
- Desarrollar validación de campos requeridos
- Integrar con la API de backend
- Escribir pruebas de componente

**Criterios de Aceptación:**
- Los formularios aparecen correctamente según la etapa destino
- La validación de campos funciona adecuadamente
- Los datos se guardan correctamente en la API
- La experiencia de usuario es fluida
- Pruebas de componente exitosas

**Dependencias:** ATS-014

**Asignado a:** Desarrollador Full-stack

**Puntos de Historia:** 8

---

## Historia de Usuario 8: Realización de evaluaciones de candidatos

### TICKET ATS-017: Diseño de interfaz para evaluación de candidatos
**Descripción:** Diseñar la interfaz de usuario para el formulario de evaluación de candidatos.

**Tareas:**
- Diseñar wireframes de formularios de evaluación
- Diseñar distintos tipos de preguntas y ratings
- Crear maquetas en alta fidelidad
- Diseñar versión móvil de los formularios
- Validar diseño con stakeholders

**Criterios de Aceptación:**
- Los formularios son intuitivos y fáciles de completar
- El diseño funciona bien en dispositivos móviles
- Soporta diferentes tipos de preguntas (escalas, texto, múltiple opción)
- Validado por stakeholders

**Dependencias:** Ninguna

**Asignado a:** Diseñador UI/UX

**Puntos de Historia:** 5

---

### TICKET ATS-018: Modelo de datos para evaluaciones
**Descripción:** Diseñar e implementar el modelo de datos para las evaluaciones de candidatos.

**Tareas:**
- Diseñar el esquema para formularios de evaluación
- Diseñar el esquema para respuestas de evaluación
- Implementar relaciones con candidatos y entrevistadores
- Configurar persistencia en MongoDB
- Escribir pruebas unitarias

**Criterios de Aceptación:**
- El modelo soporta diferentes tipos de preguntas y respuestas
- Las relaciones con candidatos y entrevistadores están correctamente establecidas
- El modelo permite análisis y consultas eficientes
- Cobertura de pruebas unitarias > 80%

**Dependencias:** ATS-012

**Asignado a:** Desarrollador Backend

**Puntos de Historia:** 5

---

### TICKET ATS-019: API REST para gestión de evaluaciones
**Descripción:** Desarrollar la API REST para la gestión de evaluaciones de candidatos.

**Tareas:**
- Implementar endpoints para crear y consultar formularios
- Desarrollar endpoints para respuestas de evaluación
- Implementar funcionalidad para adjuntar archivos
- Desarrollar endpoints para análisis de evaluaciones
- Documentar API con Swagger
- Escribir pruebas unitarias

**Criterios de Aceptación:**
- API implementada según especificaciones
- Soporte completo para gestión de formularios y respuestas
- Funcionalidad para adjuntar archivos operativa
- API documentada completamente
- Cobertura de pruebas unitarias > 80%

**Dependencias:** ATS-018

**Asignado a:** Desarrollador Backend

**Puntos de Historia:** 8

---

### TICKET ATS-020: Implementación frontend de formularios de evaluación
**Descripción:** Desarrollar los componentes frontend para completar evaluaciones de candidatos.

**Tareas:**
- Implementar formularios dinámicos basados en configuración
- Desarrollar diferentes tipos de campos (ratings, texto, selección)
- Implementar validación de campos
- Integrar con la API de backend
- Desarrollar funcionalidad para guardar borradores
- Escribir pruebas de componente

**Criterios de Aceptación:**
- Formularios implementados según diseños aprobados
- Todos los tipos de preguntas funcionan correctamente
- Los datos se guardan correctamente en la API
- La funcionalidad de borradores funciona adecuadamente
- Pruebas de componente exitosas

**Dependencias:** ATS-017, ATS-019

**Asignado a:** Desarrollador Frontend

**Puntos de Historia:** 13

---

### TICKET ATS-021: Optimización para dispositivos móviles
**Descripción:** Optimizar la experiencia de usuario de los formularios de evaluación para dispositivos móviles.

**Tareas:**
- Implementar diseño responsive para formularios
- Optimizar interacciones táctiles
- Desarrollar funcionalidad offline (opcional)
- Realizar pruebas en distintos dispositivos móviles
- Solucionar problemas específicos de móviles

**Criterios de Aceptación:**
- Los formularios funcionan correctamente en diferentes tamaños de pantalla
- La experiencia táctil es fluida y sin problemas
- La performance es adecuada en dispositivos móviles
- Funcionamiento verificado en iOS y Android

**Dependencias:** ATS-020

**Asignado a:** Desarrollador Frontend

**Puntos de Historia:** 5

---

### TICKET ATS-022: Funcionalidad para adjuntar archivos
**Descripción:** Implementar la funcionalidad para adjuntar archivos a las evaluaciones de candidatos.

**Tareas:**
- Desarrollar componente de carga de archivos
- Implementar validación de tipos y tamaños de archivo
- Integrar con servicio de almacenamiento
- Implementar gestión de permisos para archivos
- Escribir pruebas de componente

**Criterios de Aceptación:**
- La carga de archivos funciona correctamente
- Se validan los tipos y tamaños de archivos permitidos
- Los archivos se almacenan de forma segura
- Los usuarios autorizados pueden ver y descargar los archivos
- Pruebas de componente exitosas

**Dependencias:** ATS-020

**Asignado a:** Desarrollador Full-stack

**Puntos de Historia:** 5

---

### TICKET ATS-023: Pruebas de integración del flujo completo
**Descripción:** Realizar pruebas de integración del flujo completo desde la gestión de candidatos hasta la evaluación.

**Tareas:**
- Diseñar casos de prueba para flujos completos
- Implementar pruebas automatizadas end-to-end
- Realizar pruebas manuales de flujos críticos
- Probar integración entre pipeline y evaluaciones
- Documentar resultados y posibles mejoras

**Criterios de Aceptación:**
- Las pruebas cubren todos los escenarios principales y alternativos
- Todos los flujos críticos funcionan correctamente
- Se ha probado la integración entre todos los componentes
- Se han documentado todos los defectos encontrados

**Dependencias:** ATS-016, ATS-022

**Asignado a:** QA Engineer

**Puntos de Historia:** 8

---

### TICKET ATS-024: Documentación de usuario
**Descripción:** Crear documentación de usuario para los módulos de pipeline y evaluación de candidatos.

**Tareas:**
- Redactar guías de usuario para la gestión de candidatos
- Redactar guías de usuario para la evaluación de candidatos
- Crear vídeos tutoriales de los principales flujos
- Preparar materiales para capacitación

**Criterios de Aceptación:**
- La documentación cubre todas las funcionalidades implementadas
- Incluye capturas de pantalla actualizadas
- Los vídeos tutoriales son claros y muestran los flujos completos
- Revisado y aprobado por stakeholders

**Dependencias:** ATS-016, ATS-021

**Asignado a:** Technical Writer

**Puntos de Historia:** 5