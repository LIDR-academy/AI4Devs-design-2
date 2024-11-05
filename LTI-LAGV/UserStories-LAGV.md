# Documentación del Proyecto ATS

## Índice
1. [Historia de Usuario](#1-historia-de-usuario)
2. [Backlog de Producto](#2-backlog-de-producto)
3. [Tickets de Trabajo](#3-tickets-de-trabajo)
4. [Estimación del Esfuerzo de los Tickets](#4-estimación-del-esfuerzo-de-los-tickets)

---

## 1. Historia de Usuario

**Historia de Usuario 1**: Clasificación Automática de CVs  
1. Como **reclutador**  
2. quiero **que el sistema clasifique automáticamente los CVs recibidos**  
3. para que **pueda ahorrar tiempo en la revisión de aplicaciones y enfocarme en los candidatos más relevantes**.  

**Criterios de Aceptación**:  
1. El sistema debe analizar palabras clave y experiencias relevantes para clasificar los CVs.  
2. Debe permitir a los reclutadores ajustar los criterios de clasificación.  
3. Los resultados de la clasificación deben presentarse en una lista ordenada y fácil de navegar.  

---

**Historia de Usuario 2**: Automatización de Recordatorios para Entrevistas  
1. Como **reclutador**  
2. quiero **que el sistema envíe recordatorios automáticos a los candidatos sobre sus entrevistas**  
3. para que **pueda asegurarme de que los candidatos no se olviden de las citas programadas**.  

**Criterios de Aceptación**:  
1. Los recordatorios deben enviarse por email al menos 24 horas antes de la entrevista.  
2. Deben incluir información relevante como fecha, hora y lugar de la entrevista.  
3. Los reclutadores deben poder personalizar los mensajes de recordatorio.  

---

**Historia de Usuario 3**: Análisis de Tono en Entrevistas  
1. Como **reclutador**  
2. quiero **que el sistema analice el tono de las respuestas de los candidatos durante las entrevistas**  
3. para que **pueda obtener información adicional sobre su actitud y comportamiento**.  

**Criterios de Aceptación**:  
1. El sistema debe evaluar el tono de voz y las palabras utilizadas por los candidatos.  
2. Los resultados del análisis deben estar disponibles inmediatamente después de la entrevista.  
3. Debe proporcionar un resumen que identifique patrones o preocupaciones sobre el tono del candidato.  

---

**Historia de Usuario 4**: Creación de Perfiles Detallados de Candidatos  
1. Como **reclutador**  
2. quiero **crear un perfil detallado de cada candidato**  
3. para que **pueda almacenar toda la información relevante y evaluarla en cualquier momento**.  

**Criterios de Aceptación**:  
1. El perfil debe incluir datos como experiencia, habilidades, evaluaciones y anotaciones de entrevistas.  
2. Los perfiles deben poder ser actualizados en cualquier momento del proceso de selección.  
3. La información debe mostrarse en una interfaz de fácil acceso y organizada por secciones.  

---

**Historia de Usuario 5**: Panel de Control de Reclutador  
1. Como **reclutador**  
2. quiero **un panel de control con el estado de todos los procesos de selección activos**  
3. para que **pueda visualizar el progreso de cada candidato y organizar mis tareas diarias**.  

**Criterios de Aceptación**:  
1. El panel debe mostrar a todos los candidatos con su estado actual y las fases próximas.  
2. Debe incluir filtros por rol, estado del proceso, y fecha de entrevista.  
3. La información debe actualizarse automáticamente al cambiar el estado de un candidato.  

---

**Historia de Usuario 6**: Creación Automática de Respuestas para Candidatos  
1. Como **reclutador**  
2. quiero **que el sistema genere respuestas automáticas para los candidatos en cada fase del proceso**  
3. para que **pueda comunicarme con los candidatos de manera oportuna y eficiente**.  

**Criterios de Aceptación**:  
1. Las respuestas automáticas deben personalizarse con el nombre del candidato y la fase del proceso en la que se encuentra.  
2. Los mensajes deben enviarse en menos de 1 minuto después de que el candidato avance a una nueva fase.  
3. El reclutador debe poder revisar y ajustar el mensaje antes de enviarlo.  

---

**Historia de Usuario 7**: Creación de Recordatorios Automáticos para Reclutadores  
1. Como **reclutador**  
2. quiero **recibir recordatorios automáticos sobre las etapas pendientes de cada candidato**  
3. para que **pueda hacer seguimiento y no olvidar ninguna fase importante**.  

**Criterios de Aceptación**:  
1. Los recordatorios deben enviarse al menos un día antes de una actividad o fase importante.  
2. Deben poder configurarse según la fase o el rol del reclutador en el proceso.  
3. Los recordatorios deben ser visibles en el tablero principal del reclutador.  

---

**Historia de Usuario 8**: Generación de Reportes de Reclutamiento  
1. Como **manager**  
2. quiero **generar reportes sobre el desempeño del equipo de reclutamiento y el avance en los procesos**  
3. para que **pueda analizar métricas y mejorar la eficiencia del proceso de selección**.  

**Criterios de Aceptación**:  
1. Los reportes deben incluir métricas como tiempo promedio de contratación, etapas completadas y tasa de éxito.  
2. Los reportes deben ser generados en formatos PDF y Excel.  
3. Debe ser posible configurar filtros por período, tipo de puesto y reclutador.  

---

## 2. Backlog de Producto

### Tabla 1: Backlog MoSCoW

| Historia de Usuario                                                   | Prioridad (MoSCoW) |
|----------------------------------------------------------------------|---------------------|
| 1. Clasificación Automática de CVs                                   | Must Have           |
| 2. Evaluación Automatizada de Candidatos                            | Should Have         |
| 3. Chat en Vivo entre Reclutadores y Managers                       | Could Have          |
| 4. Automatización de Recordatorios para Entrevistas                  | Must Have           |
| 5. Análisis de Tono en Entrevistas                                   | Must Have           |
| 6. Creación Automática de Respuestas para Candidatos                | Should Have         |
| 7. Creación de Perfiles Detallados de Candidatos                    | Must Have           |
| 8. Creación de Recordatorios Automáticos para Reclutadores           | Should Have         |
| 9. Panel de Control de Reclutador                                    | Must Have           |
| 10. Generación de Reportes de Reclutamiento                         | Won't Have          |

### Tabla 2: Evaluación del Backlog

| Historia de Usuario                                                   | Impacto en el Usuario y Valor del Negocio | Urgencia                                | Complejidad y Esfuerzo Estimado | Riesgos y Dependencias |
|----------------------------------------------------------------------|-------------------------------------------|-----------------------------------------|----------------------------------|------------------------|
| 1. Clasificación Automática de CVs                                   | Alto                                      | Alta                                    | Alto                             | Dependiente de datos históricos |
| 2. Evaluación Automatizada de Candidatos                            | Alto                                      | Media                                   | Media                            | Integración con API de evaluación |
| 3. Chat en Vivo entre Reclutadores y Managers                       | Media                                     | Baja                                    | Baja                             | Requiere infraestructura de chat |
| 4. Automatización de Recordatorios para Entrevistas                  | Alto                                      | Alta                                    | Media                            | Dependencia del sistema de notificaciones |
| 5. Análisis de Tono en Entrevistas                                   | Alto                                      | Media                                   | Alto                             | Necesidad de procesamiento de lenguaje natural |
| 6. Creación Automática de Respuestas para Candidatos                | Media                                     | Baja                                    | Media                            | Integración con modelos de respuesta |
| 7. Creación de Perfiles Detallados de Candidatos                    | Alto                                      | Alta                                    | Media                            | Requiere acceso a datos del candidato |
| 8. Creación de Recordatorios Automáticos para Reclutadores           | Media                                     | Media                                   | Baja                             | Dependencia del sistema de recordatorios |
| 9. Panel de Control de Reclutador                                    | Alto                                      | Alta                                    | Alta                             | Necesidad de integración con varios módulos |
| 10. Generación de Reportes de Reclutamiento                         | Media                                     | Baja                                    | Media                            | Dependencia de datos recopilados |

---

## 3. Tickets de Trabajo

### **Ticket 1: Implementación del Motor de Clasificación de CVs**
- **Descripción**: Desarrollar un motor de clasificación de CVs basado en algoritmos de Machine Learning para automatizar la selección de candidatos.
- **Criterios de Aceptación**:
  - El motor debe poder clasificar CVs en diferentes categorías.
  - Debe ofrecer métricas sobre la precisión y eficiencia del modelo.
- **Prioridad**: Alta
- **Estimación**: 10 días
- **Asignado a**: Equipo de Backend
- **Etiquetas**: Machine Learning, Backend, Sprint 1
- **Comentarios**: Necesitamos validar la calidad de los datos de entrada.
- **Enlaces**: Documento de Especificación del Motor de Clasificación
- **Historial de Cambios**: 01/11/2024: Creado por [nombre]

---

### **Ticket 2: Interfaz de Usuario para Revisar Clasificación**
- **Descripción**: Crear una interfaz de usuario para que los reclutadores puedan revisar y ajustar las clasificaciones de los CVs.
- **Criterios de Aceptación**:
  - La interfaz debe ser intuitiva y fácil de navegar.
  - Permitir la edición manual de las clasificaciones.
- **Prioridad**: Alta
- **Estimación**: 7 días
- **Asignado a**: Equipo de Frontend
- **Etiquetas**: UI, Frontend, Sprint 1
- **Comentarios**: Considerar la retroalimentación de los usuarios finales.
- **Enlaces**: Prototipos de UI
- **Historial de Cambios**: 01/11/2024: Creado por [nombre]

---

### **Ticket 3: Integración con el Sistema de Notificaciones**
- **Descripción**: Integrar el motor de clasificación con el sistema de notificaciones para alertar a los reclutadores sobre nuevos candidatos clasificados.
- **Criterios de Aceptación**:
  - Notificaciones deben enviarse en tiempo real.
  - Deben ser configurables según las preferencias del usuario.
- **Prioridad**: Media
- **Estimación**: 4 días
- **Asignado a**: Equipo de Integración
- **Etiquetas**: Integración, Notificaciones, Sprint 1
- **Comentarios**: Verificar compatibilidad con sistemas de terceros.
- **Enlaces**: Documentación del Sistema de Notificaciones
- **Historial de Cambios**: 01/11/2024: Creado por [nombre]


---

### Resumen de Tickets de Trabajo

| ID  | Ticket                                            | Historia de Usuario Relacionada                                      |
|-----|--------------------------------------------------|---------------------------------------------------------------------|
| 1   | Implementación del Motor de Clasificación de CVs | Clasificación Automática de CVs (Must Have)                        |
| 2   | Desarrollo del Sistema de Recordatorios Automáticos | Automatización de Recordatorios para Entrevistas (Must Have)      |
| 3   | Integración del Análisis de Tono                 | Análisis de Tono en Entrevistas (Must Have)                       |
| 4   | Creación de Perfiles Detallados de Candidatos    | Creación de Perfiles Detallados de Candidatos (Must Have)        |
| 5   | Desarrollo del Panel de Control de Reclutador     | Panel de Control de Reclutador (Must Have)                        |
| 6   | Implementación de Evaluación Automatizada         | Evaluación Automatizada de Candidatos (Should Have)               |
| 7   | Creación de Respuestas Automáticas para Candidatos | Creación Automática de Respuestas para Candidatos (Should Have)   |
| 8   | Desarrollo de Recordatorios Automáticos para Reclutadores | Creación de Recordatorios Automáticos para Reclutadores (Should Have) |
| 9   | Implementación del Chat en Vivo                   | Chat en Vivo entre Reclutadores y Managers (Could Have)           |
| 10  | Generación de Reportes de Reclutamiento           | Generación de Reportes de Reclutamiento (Won't Have)              |


## 4. Estimación del Esfuerzo de los Tickets

### Métodos de Estimación para Tickets de Trabajo

Se utilizó una combinación de **puntos de historia** con una **escala de Fibonacci** y **tallas de camiseta** para categorizar el esfuerzo:

#### **Estimaciones Detalladas**

#### **Estimaciones Detalladas**

| ID  | Ticket                                     | Estimación (días) | Puntos de Historia | Talla de Camiseta |
|-----|--------------------------------------------|-------------------|--------------------|--------------------|
| 1   | Implementación del Motor de Clasificación   | 10                | 8                  | L                  |
| 2   | Interfaz de Usuario para Revisar Clasificación | 7                 | 5                  | M                  |
| 3   | Integración con el Sistema de Notificaciones | 4                 | 3                  | S                  |
| 4   | Desarrollo del Sistema de Recordatorios Automáticos | 5             | 5                  | M                  |
| 5   | Integración del Análisis de Tono          | 8                 | 5                  | M                  |
| 6   | Creación de Perfiles Detallados de Candidatos | 6               | 4                  | M                  |
| 7   | Desarrollo del Panel de Control de Reclutador | 12              | 8                  | L                  |
| 8   | Implementación de Evaluación Automatizada  | 9                 | 5                  | M                  |
| 9   | Creación Automática de Respuestas para Candidatos | 6           | 4                  | M                  |
| 10  | Desarrollo de Recordatorios Automáticos para Reclutadores | 5       | 3                  | S                  |
| 11  | Implementación del Chat en Vivo            | 11                | 7                  | L                  |
| 12  | Generación de Reportes de Reclutamiento    | 4                 | 2                  | S                  |


Esta documentación abarca las historias de usuario, el backlog de producto, los tickets de trabajo y la estimación del esfuerzo de cada ticket. 
