# Historias de Usuario para TalentFlow (MVP)

## Historia 1: Creación básica de vacantes

**Título**: Como reclutador, quiero crear y publicar vacantes en la plataforma para iniciar procesos de selección.

**Descripción**: Esta funcionalidad permitirá a los reclutadores crear ofertas de trabajo con la información esencial (título, descripción, requisitos, departamento, etc.) y publicarlas en la plataforma para que los candidatos puedan aplicar.

**Criterios de Aceptación**:
- Dado que soy un reclutador, cuando completo el formulario de creación de vacante con todos los campos obligatorios, entonces la vacante se crea correctamente en el sistema.
- Dado que he creado una vacante, cuando la publico, entonces se hace visible para los candidatos en la plataforma.
- Dado que tengo una vacante publicada, cuando accedo al panel de control, entonces puedo ver el estado actual de la vacante (borrador, publicada, cerrada).
- Dado que necesito modificar una vacante, cuando edito sus datos y guardo los cambios, entonces se actualizan correctamente en el sistema.

**Notas adicionales**:
- Enfocarse en la experiencia de usuario intuitiva con validación clara de campos
- Permitir guardar borradores antes de la publicación
- Implementar estados básicos para el ciclo de vida de la vacante

**Tareas**:
1. Diseñar interfaz de usuario para creación de vacantes
2. Implementar formulario de creación con campos obligatorios
3. Desarrollar funcionalidad de publicación en la plataforma
4. Implementar sistema de estados para vacantes
5. Crear capacidad de edición de vacantes
6. Realizar pruebas de usabilidad con reclutadores

## Historia 2: Búsqueda básica de candidatos

**Título**: Como reclutador, quiero buscar candidatos con criterios básicos para identificar perfiles adecuados para mis vacantes.

**Descripción**: Esta funcionalidad proporcionará a los reclutadores herramientas de búsqueda básica que les permitirán encontrar candidatos utilizando criterios simples como nombre, habilidades clave o experiencia.

**Criterios de Aceptación**:
- Dado que necesito encontrar candidatos, cuando ingreso un término de búsqueda en el campo correspondiente, entonces recibo resultados que contienen ese término en sus perfiles.
- Dado que quiero refinar mis resultados, cuando aplico filtros básicos (como nivel de experiencia o ubicación), entonces los resultados se actualizan para mostrar solo los perfiles que cumplen esos criterios.
- Dado que estoy revisando resultados de búsqueda, cuando los visualizo, entonces puedo ver información resumida relevante de cada candidato.
- Dado que quiero revisar un perfil específico, cuando hago clic en un resultado, entonces puedo acceder al perfil completo del candidato.

**Notas adicionales**:
- Priorizar la velocidad y simplicidad de la búsqueda
- Implementar filtros básicos pero efectivos
- Asegurar que el rendimiento sea bueno incluso con un número moderado de candidatos

**Tareas**:
1. Diseñar interfaz de búsqueda simple
2. Implementar motor de búsqueda básico
3. Desarrollar sistema de filtros esenciales
4. Crear vista de resultados con información resumida
5. Implementar vista detallada de perfil
6. Realizar pruebas de rendimiento básicas

## Historia 3: Experiencia de aplicación para candidatos

**Título**: Como candidato, quiero aplicar a una vacante y recibir actualizaciones sobre mi estado en el proceso de selección para mantenerme informado sobre mi progreso y próximos pasos.

**Descripción**: Esta funcionalidad permitirá a los candidatos enviar su solicitud para una vacante específica, subir o actualizar su currículum, y acceder a un panel personalizado donde podrán ver su estado actual en el proceso de selección y recibir notificaciones sobre cambios.

**Criterios de Aceptación**:
- Dado que estoy interesado en una vacante, cuando completo el formulario de aplicación y subo mi currículum, entonces recibo una confirmación de que mi solicitud ha sido recibida correctamente.
- Dado que he aplicado a una vacante, cuando accedo a mi panel de candidato, entonces puedo ver mi estado actual en el proceso de selección.
- Dado que mi estado en el proceso ha cambiado, cuando se actualiza en el sistema, entonces recibo una notificación automática informándome del cambio.
- Dado que avanzo en el proceso de selección, cuando reviso mi panel, entonces puedo ver información sobre los próximos pasos y cualquier preparación necesaria.

**Notas adicionales**:
- Diseñar la experiencia para ser accesible desde dispositivos móviles
- Asegurar que el formulario de aplicación sea simple e intuitivo
- Implementar sistema de notificaciones por correo electrónico

**Tareas**:
1. Diseñar formulario de aplicación para candidatos
2. Desarrollar sistema de subida y procesamiento de currículums
3. Implementar panel personalizado de candidato
4. Crear sistema de estados para el proceso de selección
5. Desarrollar notificaciones automáticas por correo electrónico
6. Implementar sistema de mensajes informativos sobre próximos pasos
7. Asegurar compatibilidad móvil básica
8. Realizar pruebas de usabilidad con candidatos reales

## Historia 4: Programación básica de entrevistas

**Título**: Como reclutador, quiero programar entrevistas con candidatos para avanzar en el proceso de selección.

**Descripción**: Esta funcionalidad permitirá a los reclutadores programar entrevistas con candidatos de manera sencilla, especificando fecha, hora, duración y modalidad (presencial o virtual), así como enviar invitaciones por correo electrónico.

**Criterios de Aceptación**:
- Dado que necesito programar una entrevista, cuando selecciono un candidato y accedo a la funcionalidad de programación, entonces puedo especificar fecha, hora y duración de la entrevista.
- Dado que he programado una entrevista, cuando confirmo los detalles, entonces se envía automáticamente una invitación por correo electrónico al candidato y a los entrevistadores.
- Dado que he programado varias entrevistas, cuando accedo al calendario de entrevistas, entonces puedo ver todas las entrevistas programadas.
- Dado que necesito reprogramar una entrevista, cuando modifico sus detalles y guardo los cambios, entonces se notifica automáticamente a todos los involucrados.

**Notas adicionales**:
- Enfocarse en la funcionalidad manual básica antes de implementar integraciones complejas
- Priorizar la comunicación clara con todos los participantes
- Permitir añadir notas o instrucciones específicas para la entrevista

**Tareas**:
1. Diseñar interfaz de programación de entrevistas
2. Implementar formulario de creación de entrevistas
3. Desarrollar sistema de envío de invitaciones por correo electrónico
4. Crear vista de calendario para reclutadores
5. Implementar funcionalidad de reprogramación
6. Desarrollar plantillas de correo para invitaciones
7. Realizar pruebas de flujo completo

## Historia 5: Métricas básicas para gerentes

**Título**: Como gerente de RRHH, quiero acceder a indicadores básicos de rendimiento para monitorear la efectividad del proceso de reclutamiento.

**Descripción**: Esta funcionalidad proporcionará a los gerentes de RRHH un dashboard simple con métricas clave sobre el proceso de reclutamiento, como número de vacantes activas, candidatos en proceso, y tiempo promedio de contratación.

**Criterios de Aceptación**:
- Dado que necesito supervisar el proceso de reclutamiento, cuando accedo al dashboard, entonces puedo ver el número actual de vacantes por estado (abiertas, en proceso, cerradas).
- Dado que quiero entender el flujo de candidatos, cuando reviso las métricas, entonces puedo ver el número de candidatos en cada etapa del proceso.
- Dado que necesito evaluar la eficiencia, cuando accedo a las estadísticas de tiempo, entonces puedo ver el tiempo promedio que tardan los candidatos en cada etapa.
- Dado que debo informar sobre el progreso, cuando visualizo el dashboard, entonces puedo exportar un informe básico en formato CSV.

**Notas adicionales**:
- Enfocarse en métricas esenciales que proporcionen valor inmediato
- Priorizar la claridad y simplicidad sobre la complejidad
- Asegurar que los datos se actualicen al menos diariamente

**Tareas**:
1. Diseñar dashboard simple con KPIs esenciales
2. Implementar cálculo de métricas básicas
3. Desarrollar visualizaciones simples pero efectivas
4. Crear funcionalidad de exportación básica
5. Establecer proceso de actualización periódica de datos
6. Realizar pruebas de usabilidad con gerentes

## Historia 6.1: Registro básico de candidatos

**Título**: Como reclutador, quiero registrar candidatos con su información básica para comenzar a construir mi base de datos de talento.

**Descripción**: Esta funcionalidad permitirá a los reclutadores crear perfiles básicos de candidatos con su información personal, profesional y de contacto, sentando las bases del sistema de gestión de talento.

**Criterios de Aceptación**:
- Dado que recibo un nuevo currículum, cuando creo un perfil de candidato, entonces puedo ingresar toda su información personal básica en el sistema.
- Dado que ingreso datos de un candidato, cuando completo el formulario con campos obligatorios, entonces el sistema valida y guarda correctamente la información.
- Dado que he creado varios perfiles, cuando accedo al sistema, entonces puedo ver una lista de los candidatos registrados.
- Dado que necesito verificar un perfil, cuando selecciono un candidato, entonces puedo ver toda su información básica.

**Notas adicionales**:
- Diseñar una interfaz intuitiva que facilite el ingreso rápido de datos
- Incluir validaciones claras para los campos requeridos
- Enfocar en la usabilidad para entrada rápida de datos

**Tareas**:
1. Diseñar modelo de datos para candidatos
2. Implementar base de datos para candidatos
3. Diseñar UI para formulario de creación de candidatos
4. Implementar formulario de creación de candidatos

## Historia 6.2: Visualización y búsqueda de candidatos

**Título**: Como reclutador, quiero visualizar y buscar candidatos existentes para acceder rápidamente a los perfiles relevantes.

**Descripción**: Esta funcionalidad permitirá a los reclutadores ver listados de candidatos, acceder a perfiles detallados y realizar búsquedas básicas para localizar candidatos específicos dentro del sistema.

**Criterios de Aceptación**:
- Dado que tengo candidatos registrados, cuando accedo al módulo de candidatos, entonces puedo ver una lista organizada de todos los candidatos.
- Dado que busco un candidato específico, cuando ingreso términos en el buscador, entonces recibo resultados que coinciden con mi búsqueda.
- Dado que quiero revisar información detallada, cuando hago clic en un candidato, entonces accedo a su perfil completo.
- Dado que estoy visualizando un perfil, cuando navego entre secciones, entonces puedo ver toda la información organizada de manera clara.

**Notas adicionales**:
- Priorizar la velocidad de carga de listas y perfiles
- Diseñar una interfaz limpia y fácil de navegar
- Implementar búsqueda básica eficiente

**Tareas**:
1. Creación de API para operaciones CRUD de candidatos
2. Diseño de UI para vista de detalle de candidato
3. Implementación de vista de detalle de candidato
4. Diseño de UI para lista de candidatos
5. Implementación de lista de candidatos

## Historia 6.3: Gestión de documentos de candidatos

**Título**: Como reclutador, quiero adjuntar y gestionar documentos de los candidatos para mantener sus currículums y certificaciones organizados.

**Descripción**: Esta funcionalidad permitirá a los reclutadores adjuntar, visualizar y gestionar documentos relacionados con los candidatos, como currículums, certificaciones, cartas de presentación y otros archivos relevantes.

**Criterios de Aceptación**:
- Dado que tengo un currículum de un candidato, cuando estoy en su perfil, entonces puedo adjuntar el documento al sistema.
- Dado que hay documentos adjuntos a un perfil, cuando accedo a la sección de documentos, entonces puedo ver la lista de todos los archivos disponibles.
- Dado que necesito revisar un documento, cuando selecciono uno de la lista, entonces puedo visualizarlo o descargarlo.
- Dado que un documento está desactualizado, cuando accedo a las opciones de gestión, entonces puedo eliminarlo o marcarlo como obsoleto.

**Notas adicionales**:
- Permitir formatos comunes como PDF, DOC, DOCX, JPG
- Implementar control básico de versiones
- Asegurar la seguridad de los documentos

**Tareas**:
1. Implementación de función de edición de candidatos
2. Desarrollo de sistema de almacenamiento de documentos
3. Integración de subida de documentos en formulario

## Historia 6.4: Historial y pruebas del módulo de candidatos

**Título**: Como reclutador, quiero ver un historial de cambios en los perfiles de candidatos y asegurarme que el sistema funciona correctamente.

**Descripción**: Esta funcionalidad implementará un sistema de seguimiento de cambios en los perfiles de candidatos y asegurará la calidad del módulo completo mediante pruebas exhaustivas de todos los componentes.

**Criterios de Aceptación**:
- Dado que se realizan cambios en un perfil, cuando reviso el historial, entonces puedo ver quién realizó cada cambio y cuándo.
- Dado que necesito entender modificaciones previas, cuando accedo al historial, entonces puedo ver el detalle de los cambios realizados.
- Dado que el sistema está en uso, cuando se realizan operaciones típicas, entonces todas las funcionalidades responden correctamente y sin errores.
- Dado que se añaden nuevas características, cuando se integran al sistema, entonces se mantiene la estabilidad y usabilidad de las funcionalidades existentes.

**Notas adicionales**:
- Mantener un registro detallado pero eficiente de cambios
- Realizar pruebas exhaustivas en diferentes niveles
- Documentar el funcionamiento del módulo para facilitar su uso

**Tareas**:
1. Implementación de historial básico de cambios para candidatos
2. Pruebas unitarias para módulo de candidatos
3. Pruebas de integración para módulo de candidatos
4. Pruebas de UI para módulo de candidatos
5. Documentación de uso del módulo

## Historia 7: Sistema de notificaciones

**Título**: Como usuario (candidato o reclutador), quiero recibir notificaciones por correo electrónico sobre cambios relevantes en los procesos para mantenerme informado sin necesidad de acceder constantemente al sistema.

**Descripción**: Esta funcionalidad implementará un sistema de notificaciones por correo electrónico que mantendrá informados tanto a candidatos como a reclutadores sobre eventos importantes, cambios de estado y acciones requeridas.

**Criterios de Aceptación**:
- Dado que soy un candidato, cuando mi estado en un proceso cambia, entonces recibo un correo electrónico informándome del cambio y los siguientes pasos.
- Dado que soy un reclutador, cuando un candidato aplica a una vacante, entonces recibo una notificación informándome de la nueva aplicación.
- Dado que soy un reclutador, cuando se acerca una entrevista programada, entonces recibo un recordatorio por correo electrónico.
- Dado que soy un usuario, cuando recibo un correo electrónico del sistema, entonces el mensaje es claro, profesional y contiene enlaces directos a las secciones relevantes de la plataforma.

**Notas adicionales**:
- Diseñar plantillas de correo profesionales y personalizables
- Permitir configuración básica de preferencias de notificación
- Asegurar que todos los correos incluyan enlaces directos a la acción relevante

**Tareas**:
1. Diseñar plantillas de correo electrónico para diferentes eventos
2. Implementar sistema de envío de correos
3. Desarrollar lógica de disparadores para cada tipo de notificación
4. Crear sistema básico de preferencias de notificaciones
5. Implementar proceso de validación de correos electrónicos
6. Desarrollar sistema de registro de notificaciones enviadas
7. Realizar pruebas de envío y renderizado en diferentes clientes de correo

## Backlog de Producto (Priorizado)

A continuación se presenta el backlog de producto para TalentFlow, priorizado según el análisis de impacto en usuarios, valor de negocio, urgencia, complejidad y riesgos asociados.

| ID | Historia | Impacto/Valor | Urgencia | Complejidad | Story Points | Sprint |
|----|---------|---------------|----------|-------------|--------------|--------|
| US-06.1 | Registro básico de candidatos | Alto | Alta | Media | 16 | 1 |
| US-02 | Creación básica de vacantes (parcial) | Alto | Alta | Media | 20 | 1 |
| US-06.2 | Visualización y búsqueda de candidatos | Alto | Alta | Media | 13 | 2 |
| US-02 | Creación básica de vacantes (resto) | Alto | Alta | Media | 15 | 2 |
| US-03 | Sistema de notificaciones (básico) (parcial) | Medio | Media | Baja | 15 | 2 |
| US-06.3 | Gestión de documentos de candidatos | Alto | Alta | Alta | 18 | 3 |
| US-03 | Sistema de notificaciones (básico) (resto) | Medio | Media | Baja | 21 | 3 |
| US-06.4 | Historial y pruebas del módulo de candidatos | Medio | Media | Media | 16 | 4 |
| US-04 | Experiencia de aplicación para candidatos | Alto | Alta | Alta | 34 | 5 |
| US-05 | Búsqueda básica de candidatos | Alto | Alta | Media | 28 | 6 |
| US-07 | Programación básica de entrevistas | Alto | Alta | Media | 30 | 7 |
| US-10 | Métricas básicas para gerentes | Alto | Media | Media | 25 | 8 |
| US-11 | Refinamiento y estabilización del MVP | Alto | Alta | Alta | 30 | 8 |
| US-12 | Publicación en múltiples plataformas | Alto | Media | Alta | 35 | Post-MVP |
| US-14 | Integración con calendarios corporativos | Alto | Media | Media | 25 | Post-MVP |
| US-18 | Análisis de currículums con IA | Alto | Media | Alta | 40 | Post-MVP |
| US-16 | Panel de diversidad e inclusión | Medio | Media | Media | 30 | Post-MVP |
| US-13 | Búsqueda avanzada con filtros complejos | Medio | Baja | Media | 25 | Post-MVP |
| US-15 | Reportes avanzados y análisis predictivo | Alto | Baja | Alta | 40 | Post-MVP |
| US-17 | Aplicación móvil para reclutadores | Medio | Baja | Alta | 45 | Post-MVP |

### Distribución de Sprints

#### Sprint 1: Base del Sistema (36 Story Points)
**Objetivo**: Implementar el registro básico de candidatos y comenzar la creación básica de vacantes.

| ID | Historia | Story Points | Prioridad |
|----|---------|--------------|-----------|
| US-06.1 | Registro básico de candidatos | 16 SP | Must Have |
| US-02 (parcial) | Creación básica de vacantes (primera parte) | 20 SP | Must Have |

#### Sprint 2: Visualización y Búsqueda (43 Story Points)
**Objetivo**: Completar la visualización de candidatos, terminar la creación de vacantes e iniciar las notificaciones.

| ID | Historia | Story Points | Prioridad |
|----|---------|--------------|-----------|
| US-06.2 | Visualización y búsqueda de candidatos | 13 SP | Must Have |
| US-02 (resto) | Creación básica de vacantes (finalización) | 15 SP | Must Have |
| US-03 (parcial) | Sistema de notificaciones (inicio) | 15 SP | Should Have |

#### Sprint 3: Gestión de Documentos (39 Story Points)
**Objetivo**: Implementar la gestión de documentos de candidatos y completar el sistema de notificaciones.

| ID | Historia | Story Points | Prioridad |
|----|---------|--------------|-----------|
| US-06.3 | Gestión de documentos de candidatos | 18 SP | Must Have |
| US-03 (resto) | Sistema de notificaciones (finalización) | 21 SP | Should Have |

#### Sprint 4: Consolidación del Módulo de Candidatos (41 Story Points)
**Objetivo**: Completar, probar y estabilizar el módulo de candidatos e iniciar la configuración de infraestructura.

| ID | Historia | Story Points | Prioridad |
|----|---------|--------------|-----------|
| US-06.4 | Historial y pruebas del módulo de candidatos | 16 SP | Must Have |
| Tickets transversales | Infraestructura, autenticación y componentes base | 25 SP | Must Have |

## Tickets de Trabajo para Sprint 1

A continuación se detallan los tickets de trabajo con sus estimaciones para el Sprint 1:

### US-06.1: Registro básico de candidatos (16 SP)

| ID Ticket | Descripción | Story Points | Tipo | Componente |
|-----------|-------------|--------------|------|------------|
| TF-101 | Diseño de modelo de datos para candidatos | 5 SP | Diseño | Backend |
| TF-102 | Implementación de base de datos para candidatos | 3 SP | Desarrollo | Backend |
| TF-104 | Diseño de UI para formulario de creación de candidatos | 3 SP | Diseño | Frontend |
| TF-105 | Implementación de formulario de creación de candidatos | 5 SP | Desarrollo | Frontend |

### US-02: Creación básica de vacantes (parcial) (20 SP)

| ID Ticket | Descripción | Story Points | Tipo | Componente |
|-----------|-------------|--------------|------|------------|
| TF-201 | Diseño de modelo de datos para vacantes | 3 SP | Diseño | Backend |
| TF-202 | Implementación de base de datos para vacantes | 2 SP | Desarrollo | Backend |
| TF-203 | Creación de API para operaciones CRUD de vacantes | 3 SP | Desarrollo | Backend |
| TF-204 | Implementación de sistema de estados para vacantes | 5 SP | Desarrollo | Backend |
| TF-205 | Diseño de UI para formulario de creación de vacantes | 2 SP | Diseño | Frontend |
| TF-206 | Implementación de formulario de creación de vacantes | 3 SP | Desarrollo | Frontend |
| TF-207 | Desarrollo de funcionalidad de publicación de vacantes | 2 SP | Desarrollo | Backend |

### Tickets para Sprint 2 (Pre-planificación)

#### US-06.2: Visualización y búsqueda de candidatos (13 SP)

| ID Ticket | Descripción | Story Points | Tipo | Componente |
|-----------|-------------|--------------|------|------------|
| TF-103 | Creación de API para operaciones CRUD de candidatos | 5 SP | Desarrollo | Backend |
| TF-106 | Diseño de UI para vista de detalle de candidato | 2 SP | Diseño | Frontend |
| TF-107 | Implementación de vista de detalle de candidato | 3 SP | Desarrollo | Frontend |
| TF-108 | Diseño de UI para lista de candidatos | 2 SP | Diseño | Frontend |
| TF-109 | Implementación de lista de candidatos | 3 SP | Desarrollo | Frontend |

#### US-02: Creación básica de vacantes (resto) (15 SP)

| ID Ticket | Descripción | Story Points | Tipo | Componente |
|-----------|-------------|--------------|------|------------|
| TF-208 | Diseño de UI para panel de control de vacantes | 2 SP | Diseño | Frontend |
| TF-209 | Implementación de panel de control de vacantes | 3 SP | Desarrollo | Frontend |
| TF-210 | Implementación de función de edición de vacantes | 3 SP | Desarrollo | Frontend |
| TF-211 | Pruebas unitarias para módulo de vacantes | 2 SP | Testing | Backend |
| TF-212 | Pruebas de integración para módulo de vacantes | 2 SP | Testing | QA |
| TF-213 | Pruebas de UI para módulo de vacantes | 3 SP | Testing | QA |

#### US-03: Sistema de notificaciones (parcial) (15 SP)

| ID Ticket | Descripción | Story Points | Tipo | Componente |
|-----------|-------------|--------------|------|------------|
| TF-301 | Diseño de arquitectura para sistema de notificaciones | 5 SP | Diseño | Backend |
| TF-302 | Configuración de servicio de envío de correos | 3 SP | Desarrollo | DevOps |
| TF-303 | Diseño de plantillas de correo para eventos clave | 2 SP | Diseño | Frontend |
| TF-304 | Desarrollo de servicio de envío de correos | 5 SP | Desarrollo | Backend |

### Tickets para Sprint 3 (Pre-planificación)

#### US-06.3: Gestión de documentos de candidatos (18 SP)

| ID Ticket | Descripción | Story Points | Tipo | Componente |
|-----------|-------------|--------------|------|------------|
| TF-110 | Implementación de función de edición de candidatos | 5 SP | Desarrollo | Frontend |
| TF-111 | Desarrollo de sistema de almacenamiento de documentos | 8 SP | Desarrollo | Backend |
| TF-112 | Integración de subida de documentos en formulario | 5 SP | Desarrollo | Frontend |

#### US-03: Sistema de notificaciones (resto) (21 SP)

| ID Ticket | Descripción | Story Points | Tipo | Componente |
|-----------|-------------|--------------|------|------------|
| TF-305 | Implementación de disparadores básicos de notificaciones | 5 SP | Desarrollo | Backend |
| TF-306 | Integración de notificaciones con módulo de candidatos | 3 SP | Desarrollo | Backend |
| TF-307 | Integración de notificaciones con módulo de vacantes | 2 SP | Desarrollo | Backend |
| TF-308 | Sistema de registro de notificaciones enviadas | 3 SP | Desarrollo | Backend |
| TF-309 | Pruebas unitarias para módulo de notificaciones | 2 SP | Testing | Backend |
| TF-310 | Pruebas de integración para módulo de notificaciones | 3 SP | Testing | QA |
| TF-311 | Pruebas de entrega de correos en diferentes entornos | 3 SP | Testing | QA |

### Tickets para Sprint 4 (Pre-planificación)

#### US-06.4: Historial y pruebas del módulo de candidatos (16 SP)

| ID Ticket | Descripción | Story Points | Tipo | Componente |
|-----------|-------------|--------------|------|------------|
| TF-113 | Implementación de historial básico de cambios | 5 SP | Desarrollo | Backend |
| TF-114 | Pruebas unitarias para módulo de candidatos | 3 SP | Testing | Backend |
| TF-115 | Pruebas de integración para módulo de candidatos | 3 SP | Testing | QA |
| TF-116 | Pruebas de UI para módulo de candidatos | 3 SP | Testing | QA |
| TF-117 | Documentación de uso del módulo de candidatos | 2 SP | Documentación | Gestión |

#### Tickets transversales prioritarios (25 SP)

| ID Ticket | Descripción | Story Points | Tipo | Componente |
|-----------|-------------|--------------|------|------------|
| TF-401 | Configuración inicial de proyecto (estructura, CI/CD) | 8 SP | DevOps | Infraestructura |
| TF-402 | Configuración de entornos (desarrollo, testing, staging) | 5 SP | DevOps | Infraestructura |
| TF-403 | Implementación de autenticación y autorización básica | 8 SP | Desarrollo | Backend |
| TF-404 | Desarrollo de componentes UI reutilizables | 5 SP | Desarrollo | Frontend |
| TF-405 | Implementación de navegación principal y layout base | 3 SP | Desarrollo | Frontend |
| TF-406 | Sesiones de revisión con stakeholders | 1 SP | Análisis | Gestión |
| TF-407 | Documentación técnica de componentes | 3 SP | Documentación | Gestión |
| TF-408 | Preparación de demo para revisión de sprint | 2 SP | Gestión | Gestión |
