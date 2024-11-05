
# Historias de Usuario - LTI ATS

## 1. Gestión de Usuarios y Roles

### Historia de Usuario 1: Creación de Cuentas y Asignación de Roles

1. **Como** Administrador,
2. **quiero** crear nuevas cuentas de usuario y asignarles un rol específico (Candidato, Reclutador, Gerente de Contratación, Analista de Datos, Coordinador de Procesos),
3. **para que** cada usuario tenga acceso a las funcionalidades adecuadas según su rol en el ATS.

**Criterios de Aceptación**:

1. El sistema debe permitir la creación de cuentas mediante un formulario, solicitando información obligatoria como nombre, correo electrónico y rol asignado.
2. Al crear la cuenta, el sistema debe enviar un correo de bienvenida al usuario con instrucciones para acceder al ATS.
3. El rol asignado debe definir automáticamente los permisos y accesos dentro del sistema.
4. El administrador debe poder editar el rol de un usuario existente en caso de cambio de responsabilidades.

**Notas Adicionales**:

- La creación de cuentas debe seguir políticas de seguridad que aseguren que solo los administradores pueden realizar esta acción.
- La lista de roles debe estar predefinida en el sistema para evitar errores en la asignación de permisos.

**Historias de Usuario Relacionadas**:

- **Historia 2**: Definición de permisos específicos para cada rol.
- **Historia 3**: Auditoría de actividades por usuario.

---

### Historia de Usuario 2: Definición de Permisos por Rol

1. **Como** Administrador,
2. **quiero** definir permisos específicos para cada rol en el sistema,
3. **para que** los usuarios solo puedan realizar las acciones autorizadas dentro de su rol, asegurando seguridad y control en el acceso a funcionalidades.

**Criterios de Aceptación**:

1. El sistema debe permitir al administrador visualizar una lista de roles y los permisos asociados a cada uno.
2. Cada rol debe tener permisos definidos para el acceso a módulos como "Gestión de Vacantes", "Análisis de Datos", "Programación de Entrevistas", entre otros.
3. El sistema debe restringir automáticamente el acceso de los usuarios según el rol asignado, mostrando solo las funcionalidades permitidas.

**Notas Adicionales**:

- Los permisos deben ser configurables para adaptarse a cambios organizacionales o personalización de la plataforma.
- Las restricciones de acceso deben actualizarse en tiempo real si el rol de un usuario cambia.

**Historias de Usuario Relacionadas**:

- **Historia 1**: Creación de cuentas y asignación de roles.
- **Historia 3**: Auditoría de actividades por usuario.

---

### Historia de Usuario 3: Auditoría de Actividades por Usuario

1. **Como** Administrador,
2. **quiero** auditar las actividades de cada usuario según su rol y permisos,
3. **para que** pueda monitorear el uso del sistema, detectar accesos no autorizados y asegurar el cumplimiento de políticas internas.

**Criterios de Aceptación**:

1. El sistema debe generar un registro de actividades por usuario, que incluya información detallada como fecha, hora, tipo de acción realizada y resultado.
2. Solo los administradores deben tener acceso a estos registros de actividad.
3. El sistema debe permitir la exportación de los registros en formato CSV para auditorías externas o análisis detallado.

**Notas Adicionales**:

- Los registros de actividad deben almacenarse de forma segura y cumplir con las normativas de protección de datos.
- Debe incluirse una función de búsqueda y filtrado en los registros para facilitar la revisión de actividades específicas.

**Historias de Usuario Relacionadas**:

- **Historia 1**: Creación de cuentas y asignación de roles.
- **Historia 2**: Definición de permisos por rol.

---

## 2. Creación y Publicación de Vacantes

### Historia de Usuario 1: Creación de Nueva Vacante

1. **Como** Reclutador,
2. **quiero** crear una nueva vacante en el sistema ingresando información relevante (título del puesto, descripción, requisitos, ubicación, etc.),
3. **para que** pueda gestionar y publicar ofertas de trabajo de manera centralizada.

**Criterios de Aceptación**:

1. El sistema debe ofrecer un formulario de creación de vacante con campos obligatorios y opcionales (título, descripción, requisitos, ubicación, tipo de contrato, salario, etc.).
2. El reclutador debe poder guardar la vacante como borrador antes de publicarla para revisarla y hacer cambios.
3. Al guardar la vacante, el sistema debe validar que todos los campos obligatorios estén completos y mostrar un mensaje de confirmación al reclutador.

**Notas Adicionales**:

- La vacante debe asignarse automáticamente a la cuenta del reclutador que la creó para facilitar la trazabilidad.
- Los borradores deben estar disponibles en una sección de "Vacantes Guardadas" para un acceso rápido.

**Historias de Usuario Relacionadas**:

- **Historia 2**: Publicación de vacante en plataformas externas.
- **Historia 3**: Edición y actualización de vacantes.

---

### Historia de Usuario 2: Publicación de Vacante en Plataformas Externas

1. **Como** Reclutador,
2. **quiero** publicar una vacante en plataformas de empleo externas (LinkedIn, Indeed, etc.) desde el sistema,
3. **para que** pueda aumentar la visibilidad de la oferta y atraer más candidatos.

**Criterios de Aceptación**:

1. El sistema debe permitir al reclutador seleccionar las plataformas en las que desea publicar la vacante.
2. Al seleccionar una plataforma, el sistema debe proporcionar opciones para personalizar el contenido de la publicación, adaptándolo a los requisitos de cada plataforma.
3. El reclutador debe recibir una notificación de confirmación cuando la vacante se haya publicado exitosamente en las plataformas seleccionadas.

**Notas Adicionales**:

- Las integraciones con plataformas externas deben estar configuradas para que el proceso de publicación sea automático y sin fricciones.
- El sistema debe mostrar el estado de publicación (publicada, pendiente, fallida) para cada plataforma seleccionada.

**Historias de Usuario Relacionadas**:

- **Historia 1**: Creación de nueva vacante.
- **Historia 3**: Edición y actualización de vacantes.

---

### Historia de Usuario 3: Edición y Actualización de Vacantes

1. **Como** Reclutador,
2. **quiero** editar y actualizar la información de una vacante después de haberla publicado,
3. **para que** pueda reflejar cualquier cambio en los requisitos o detalles del puesto en tiempo real.

**Criterios de Aceptación**:

1. El reclutador debe poder acceder a las vacantes publicadas y realizar ediciones en todos los campos (descripción, requisitos, ubicación, etc.).
2. El sistema debe notificar al reclutador que las actualizaciones pueden demorar en reflejarse en las plataformas externas.
3. Si la vacante está en proceso de contratación, el sistema debe mostrar una advertencia sobre el impacto de los cambios en los candidatos actuales.

**Notas Adicionales**:

- Las actualizaciones en vacantes publicadas deben sincronizarse con las plataformas externas.
- Un historial de cambios debe mantenerse para cada vacante, incluyendo la fecha, hora y detalles de cada modificación.

**Historias de Usuario Relacionadas**:

- **Historia 1**: Creación de nueva vacante.
- **Historia 2**: Publicación de vacante en plataformas externas.

---

## 3. Aplicación y Seguimiento de Candidatos

### Historia de Usuario 1: Aplicación a una Vacante

1. **Como** Candidato,
2. **quiero** aplicar a una vacante disponible en el sistema,
3. **para que** pueda postularme a oportunidades laborales que coincidan con mi perfil profesional.

**Criterios de Aceptación**:

1. El candidato debe poder acceder a la lista de vacantes activas y seleccionar una para ver los detalles.
2. El sistema debe proporcionar un formulario de aplicación que incluya campos como información personal, carga de CV y campo opcional para carta de presentación.
3. Al completar la aplicación, el sistema debe mostrar una confirmación de envío y enviar una notificación al correo del candidato.

**Notas Adicionales**:

- El sistema debe validar que los campos obligatorios estén completos antes de permitir el envío de la aplicación.
- El candidato debe tener la opción de guardar la vacante como favorita para aplicar en otro momento.

**Historias de Usuario Relacionadas**:

- **Historia 2**: Seguimiento del estado de la aplicación.
- **Historia 3**: Evaluación inicial de candidatos por el reclutador.

---

### Historia de Usuario 2: Seguimiento del Estado de la Aplicación

1. **Como** Candidato,
2. **quiero** ver el estado de mi aplicación en cada etapa del proceso de selección,
3. **para que** pueda estar informado sobre el progreso y la situación de mi candidatura.

**Criterios de Aceptación**:

1. El sistema debe mostrar un tablero de seguimiento que incluya las etapas del proceso de selección (aplicación recibida, en revisión, entrevista programada, oferta, etc.).
2. El candidato debe recibir notificaciones de actualización cada vez que su aplicación cambie de estado.
3. El candidato debe poder retirar su aplicación en cualquier momento, recibiendo una confirmación de cancelación.

**

Notas Adicionales**:

- Las actualizaciones de estado deben ser automáticas y en tiempo real, reflejando las acciones de los reclutadores.
- Los mensajes de estado deben ser claros y en lenguaje amigable para el candidato.

**Historias de Usuario Relacionadas**:

- **Historia 1**: Aplicación a una vacante.
- **Historia 3**: Evaluación inicial de candidatos por el reclutador.

---

### Historia de Usuario 3: Evaluación Inicial de Candidatos por el Reclutador

1. **Como** Reclutador,
2. **quiero** realizar una evaluación inicial de los candidatos que han aplicado a una vacante,
3. **para que** pueda identificar a los perfiles más adecuados para avanzar en el proceso de selección.

**Criterios de Aceptación**:

1. El reclutador debe poder acceder a la lista de aplicaciones recibidas y visualizar el perfil completo de cada candidato (CV, carta de presentación, experiencia relevante, etc.).
2. El sistema debe permitir al reclutador marcar a los candidatos como "preseleccionados" o "rechazados" en esta etapa inicial.
3. El reclutador debe poder añadir notas y comentarios en el perfil del candidato para referencia en futuras etapas.

**Notas Adicionales**:

- Los candidatos rechazados deben recibir una notificación automática indicando que su perfil no ha sido seleccionado para la vacante.
- El sistema debe registrar y almacenar cualquier comentario o nota realizada por el reclutador.

**Historias de Usuario Relacionadas**:

- **Historia 1**: Aplicación a una vacante.
- **Historia 2**: Seguimiento del estado de la aplicación.

---

## 4. Programación de Entrevistas

### Historia de Usuario 1: Programación de Entrevistas Automática

1. **Como** Reclutador,
2. **quiero** programar entrevistas para los candidatos seleccionados,
3. **para que** pueda coordinar las entrevistas de forma automática y sin conflictos de horario.

**Criterios de Aceptación**:

1. El reclutador debe poder seleccionar una fecha y hora sugerida para la entrevista de acuerdo con la disponibilidad del candidato y del entrevistador.
2. El sistema debe sincronizarse con los calendarios de Google Calendar y Outlook para evitar conflictos de horario.
3. Al confirmar la programación, el sistema debe enviar notificaciones automáticas tanto al candidato como al entrevistador con los detalles de la entrevista.

**Notas Adicionales**:

- El sistema debe permitir que el reclutador elija entre opciones de entrevista presencial o virtual, proporcionando un enlace de videoconferencia cuando sea necesario.
- Las notificaciones deben incluir la opción para reprogramar o cancelar la entrevista si fuera necesario.

**Historias de Usuario Relacionadas**:

- **Historia 2**: Recordatorios automáticos de entrevistas.
- **Historia 3**: Registro de feedback post-entrevista.

---

### Historia de Usuario 2: Recordatorios Automáticos de Entrevistas

1. **Como** Coordinador de Procesos,
2. **quiero** que el sistema envíe recordatorios automáticos de entrevistas a candidatos y entrevistadores,
3. **para que** todos estén puntualmente informados y preparados para cada entrevista.

**Criterios de Aceptación**:

1. El sistema debe enviar recordatorios automáticos al candidato y al entrevistador un día antes y una hora antes de la entrevista programada.
2. Los recordatorios deben incluir el enlace de videoconferencia o la ubicación de la entrevista si es presencial.
3. El sistema debe permitir al candidato y al entrevistador confirmar su asistencia o solicitar una reprogramación desde el recordatorio.

**Notas Adicionales**:

- Los recordatorios deben ser personalizables en términos de tiempo (p. ej., enviar notificaciones adicionales con 3 horas de anticipación si es necesario).
- Las notificaciones deben incluir todos los detalles relevantes de la entrevista para evitar confusiones.

**Historias de Usuario Relacionadas**:

- **Historia 1**: Programación de entrevistas automática.
- **Historia 3**: Registro de feedback post-entrevista.

---

### Historia de Usuario 3: Registro de Feedback Post-Entrevista

1. **Como** Reclutador,
2. **quiero** registrar el feedback y las evaluaciones de los entrevistadores después de cada entrevista,
3. **para que** pueda tomar decisiones informadas y coordinadas sobre la selección de candidatos.

**Criterios de Aceptación**:

1. El sistema debe permitir al reclutador y a los entrevistadores añadir notas y puntuaciones en el perfil del candidato después de cada entrevista.
2. El feedback debe ser visible únicamente para el equipo de reclutamiento y los gerentes de contratación, manteniendo la confidencialidad de los comentarios.
3. Los comentarios y las evaluaciones deben ser editables dentro de un período de 24 horas después de la entrevista, y luego ser almacenados como registros definitivos.

**Notas Adicionales**:

- Debe existir una funcionalidad para visualizar el historial de feedback de todas las entrevistas del candidato en el proceso de selección.
- La interfaz de feedback debe ser intuitiva, permitiendo puntuaciones y comentarios detallados de manera rápida y eficaz.

**Historias de Usuario Relacionadas**:

- **Historia 1**: Programación de entrevistas automática.
- **Historia 2**: Recordatorios automáticos de entrevistas.


---
---

# Backlog de Producto - LTI ATS

## Fase 1: Gestión de Usuarios y Roles

| ID     | Historia de Usuario                                 | Prioridad | Sprint Propuesto | Dependencias                                | Notas Adicionales                              |
|--------|-----------------------------------------------------|-----------|------------------|---------------------------------------------|------------------------------------------------|
| USR-01 | Creación de Cuentas y Asignación de Roles           | Alta      | Sprint 1         | Ninguna                                     | Incluye validación de seguridad.               |
| USR-02 | Definición de Permisos por Rol                      | Alta      | Sprint 1         | USR-01                                      | Configurable en tiempo real.                   |
| USR-03 | Auditoría de Actividades por Usuario                | Media     | Sprint 2         | USR-02                                      | Cumple con normas de protección de datos.      |

---

## Fase 2: Creación y Publicación de Vacantes

| ID     | Historia de Usuario                                 | Prioridad | Sprint Propuesto | Dependencias                                | Notas Adicionales                              |
|--------|-----------------------------------------------------|-----------|------------------|---------------------------------------------|------------------------------------------------|
| VAC-01 | Creación de Nueva Vacante                           | Alta      | Sprint 1         | Ninguna                                     | Requiere campos obligatorios y opcionales.     |
| VAC-02 | Publicación de Vacante en Plataformas Externas      | Media     | Sprint 2         | VAC-01                                      | Integraciones externas con bolsas de trabajo.  |
| VAC-03 | Edición y Actualización de Vacantes                 | Media     | Sprint 2         | VAC-01                                      | Mantiene historial de cambios.                 |

---

## Fase 3: Aplicación y Seguimiento de Candidatos

| ID     | Historia de Usuario                                 | Prioridad | Sprint Propuesto | Dependencias                                | Notas Adicionales                              |
|--------|-----------------------------------------------------|-----------|------------------|---------------------------------------------|------------------------------------------------|
| CAN-01 | Aplicación a una Vacante                            | Alta      | Sprint 1         | VAC-01                                      | Permite guardar vacantes como favoritas.       |
| CAN-02 | Seguimiento del Estado de la Aplicación             | Alta      | Sprint 1         | CAN-01                                      | Actualización de estado en tiempo real.        |
| CAN-03 | Evaluación Inicial de Candidatos por el Reclutador  | Alta      | Sprint 1         | CAN-01                                      | Incluye notificaciones automáticas a candidatos.|

---

## Fase 4: Programación de Entrevistas

| ID     | Historia de Usuario                                 | Prioridad | Sprint Propuesto | Dependencias                                | Notas Adicionales                              |
|--------|-----------------------------------------------------|-----------|------------------|---------------------------------------------|------------------------------------------------|
| ENT-01 | Programación de Entrevistas Automática              | Alta      | Sprint 2         | CAN-03                                      | Sincronización con calendarios externos.       |
| ENT-02 | Recordatorios Automáticos de Entrevistas            | Media     | Sprint 2         | ENT-01                                      | Incluye opción de reprogramar.                 |
| ENT-03 | Registro de Feedback Post-Entrevista                | Alta      | Sprint 3         | ENT-01                                      | Feedback visible solo para equipo de reclutamiento.|

---
**NOTA**:
Se crearon los tickets de trabajo solo para las historias de usuario de la fase 1.

---
## Tickets de Trabajo: Gestión de Usuarios y Roles


### Ticket 1: Creación de Cuentas y Asignación de Roles

- **ID**: USR-01
- **Tipo**: Característica (Feature)
- **Título**: Implementación de Creación de Cuentas y Asignación de Roles
- **Descripción**:
  - **Propósito**: Permitir al administrador crear cuentas para nuevos usuarios en el sistema y asignar roles específicos (Candidato, Reclutador, Gerente de Contratación, Analista de Datos, Coordinador de Procesos). Esta funcionalidad asegura que cada usuario tenga permisos y accesos correspondientes a su rol.
  - **Detalles Específicos**: Incluir un formulario de registro con campos obligatorios, como nombre, correo electrónico y rol asignado. Al crear la cuenta, el sistema enviará automáticamente un correo de bienvenida al usuario.

**Criterios de Aceptación**:
- El administrador puede crear cuentas de usuario mediante un formulario que incluya nombre, correo electrónico y rol.
- El sistema valida que todos los campos obligatorios estén completos antes de permitir la creación de la cuenta.
- Al crear la cuenta, el sistema envía automáticamente un correo de bienvenida al usuario.
- El rol asignado define los permisos de acceso en el sistema.
- El administrador puede editar el rol de un usuario existente.

**Prioridad**: Alta  
**Asignación**: Equipo de Backend y Equipo de UI  
**Etiquetas**: Gestión de Usuarios, Seguridad, Backend, Sprint 1  

**Comentarios y Notas**:
- Asegurarse de que solo los administradores puedan crear cuentas, siguiendo los principios de seguridad de acceso.
- Configurar una plantilla de correo de bienvenida con instrucciones para el usuario sobre cómo acceder al sistema.

**Enlaces o Referencias**:
- Documentación de Roles y Permisos de Usuario

**Historial de Cambios**:
- 03/11/2024: Ticket creado.

---

### Ticket 2: Definición de Permisos por Rol

- **ID**: USR-02
- **Tipo**: Característica (Feature)
- **Título**: Configuración de Permisos por Rol
- **Descripción**:
  - **Propósito**: Configurar permisos específicos para cada rol en el sistema, de manera que los usuarios solo puedan realizar las acciones autorizadas dentro de su rol, garantizando así la seguridad y control de acceso.
  - **Detalles Específicos**: Cada rol tendrá permisos asignados para acceso a diferentes módulos (como "Gestión de Vacantes", "Análisis de Datos", etc.). El administrador podrá visualizar y, si es necesario, actualizar los permisos asignados a cada rol.

**Criterios de Aceptación**:
- El administrador puede visualizar una lista de roles y los permisos específicos asignados a cada uno.
- Los permisos definidos limitan el acceso de los usuarios, mostrando solo las funcionalidades permitidas para cada rol.
- Los cambios en los permisos se reflejan en tiempo real si el rol de un usuario cambia.

**Prioridad**: Alta  
**Asignación**: Equipo de Backend  
**Etiquetas**: Gestión de Usuarios, Seguridad, Backend, Sprint 1  

**Comentarios y Notas**:
- Asegurar que los permisos sean configurables para adaptarse a cambios organizacionales.
- Validar que los permisos estén alineados con la política de seguridad de la plataforma.

**Enlaces o Referencias**:
- Documentación sobre Roles y Permisos.

**Historial de Cambios**:
- 03/11/2024: Ticket creado.

---

### Ticket 3: Auditoría de Actividades por Usuario

- **ID**: USR-03
- **Tipo**: Característica (Feature)
- **Título**: Implementación de Auditoría de Actividades de Usuario
- **Descripción**:
  - **Propósito**: Crear un registro de auditoría que permita a los administradores monitorear y auditar las acciones realizadas por cada usuario, cumpliendo con políticas de seguridad y normativas de protección de datos.
  - **Detalles Específicos**: El sistema debe almacenar actividades clave realizadas por el usuario, incluyendo información detallada como fecha, hora, tipo de acción y resultado. Solo los administradores tendrán acceso a este registro.

**Criterios de Aceptación**:
- El sistema genera un registro de actividades que incluye información detallada como fecha, hora, tipo de acción realizada y resultado.
- Solo los administradores pueden acceder al registro de actividades.
- El sistema permite la exportación del registro en formato CSV.

**Prioridad**: Media  
**Asignación**: Equipo de Backend y QA  
**Etiquetas**: Auditoría, Seguridad, Backend, Sprint 2  

**Comentarios y Notas**:
- Asegurarse de que los registros de actividad se almacenan de manera segura y cumplen con las regulaciones de protección de datos.
- Incluir una opción de búsqueda y filtrado en el registro para facilitar la revisión de actividades específicas.

**Enlaces o Referencias**:
- Documentación de Auditoría y Normativas de Protección de Datos.

**Historial de Cambios**:
- 03/11/2024: Ticket creado.

---

### Ticket 4: Integración de Roles en el Sistema de Autenticación

- **ID**: USR-04
- **Tipo**: Tarea Técnica
- **Título**: Configuración de Roles en el Sistema de Autenticación y Control de Acceso
- **Descripción**:
  - **Propósito**: Asegurar que el sistema de autenticación restrinja el acceso de los usuarios a las funcionalidades permitidas de acuerdo con su rol. Esta integración garantiza que cada usuario solo pueda acceder a las áreas y acciones asignadas a su perfil.
  - **Detalles Específicos**: Configurar autenticación basada en roles, de modo que el acceso se ajuste inmediatamente si el rol de un usuario cambia. Validar que el sistema de autenticación funcione correctamente para cada rol.

**Criterios de Aceptación**:
- El sistema de autenticación verifica el rol del usuario antes de otorgar acceso a cada módulo o funcionalidad.
- Los usuarios solo pueden acceder a las secciones y acciones permitidas para su rol.
- Si el rol de un usuario cambia, el acceso se actualiza inmediatamente en el sistema.

**Prioridad**: Alta  
**Asignación**: Equipo de Backend  
**Etiquetas**: Autenticación, Seguridad, Backend, Sprint 1  

**Comentarios y Notas**:
- Configurar autenticación basada en roles para mejorar la seguridad del sistema.
- Realizar pruebas exhaustivas para verificar que cada rol tiene los permisos correctos y no puede acceder a secciones no autorizadas.

**Enlaces o Referencias**:
- Documentación de Roles y Autenticación.

**Historial de Cambios**:
- 03/11/2024: Ticket creado.

---
---

## Estimación de Esfuerzo: Planning Poker

| ID     | Nombre                                           | Puntos de Estimación | Sprint Asignado | Prioridad | Descripción del Esfuerzo                                                                                                                                           |
|--------|--------------------------------------------------|-----------------------|-----------------|-----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| USR-01 | Implementación de Creación de Cuentas y Asignación de Roles | 5                     | Sprint 1       | Alta      | Complejidad moderada debido a la validación de roles, creación de cuentas y envío de correos de bienvenida. La lógica de asignación requiere pruebas adicionales.   |
| USR-02 | Configuración de Permisos por Rol                | 2                     | Sprint 1       | Alta      | Baja complejidad, ya que se basa en una lista predefinida de permisos que el administrador puede visualizar y editar en tiempo real.                                |
| USR-03 | Implementación de Auditoría de Actividades de Usuario | 8                     | Sprint 2       | Media     | Alta complejidad, debido a la necesidad de almacenar y gestionar un registro de actividades seguro y exportable, con opción de búsqueda y cumplimiento de normativas. |
| USR-04 | Configuración de Roles en el Sistema de Autenticación | 5                     | Sprint 1       | Alta      | Complejidad técnica media debido a la integración con el sistema de autenticación y el control de acceso en tiempo real según los roles asignados.                 |

---
