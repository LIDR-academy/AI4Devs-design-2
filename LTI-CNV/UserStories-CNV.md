
# ------------- USER STORIES ------------- ###


# 1. Filtrado de Candidatos

## User Story

**Como Reclutador**, quiero filtrar candidatos por palabras clave, ubicación y experiencia para encontrar rápidamente a los más adecuados para la vacante.

## Descripción

El reclutador dispondrá de una sección o panel donde pueda aplicar filtros avanzados (por ejemplo, años de experiencia, palabras clave, ubicación). De esta manera, podrá reducir la lista de candidatos y centrarse en los que mejor encajan con los requisitos de la oferta.

## Criterios de Aceptación

- **Dado** que el reclutador se encuentra en la lista de candidatos,  
  **cuando** aplique uno o varios filtros (por ejemplo, "Java", "3 años de experiencia", "Madrid"),  
  **entonces** el sistema mostrará únicamente los candidatos que cumplan con todos esos criterios.

- **Dado** que existan más de 100 candidatos,  
  **cuando** el reclutador aplique filtros y pagine la lista,  
  **entonces** se deberá mostrar la paginación y el número total de resultados filtrados.

## Notas Adicionales

- Se recomienda implementar paginación y ordenamiento para un rendimiento óptimo en grandes volúmenes de datos.
- Los filtros deben poder combinarse (palabra clave + ubicación + experiencia).

## Tareas

- **Diseño de UI:** Crear la interfaz de filtrado (campos, menús desplegables, etc.).
- **Implementación de lógica:** Ajustar el endpoint de búsqueda en la API para recibir parámetros de filtrado.
- **Validar resultados:** Asegurar que la API devuelva solo los candidatos que cumplan los criterios.
- **Paginación:** Implementar paginación y ordenamiento en el resultado.
- **Pruebas:** Realizar pruebas de carga y funcionales con distintos volúmenes de datos.

---

# 2. Programación de Entrevistas

## User Story

**Como Reclutador**, quiero programar entrevistas con los candidatos preseleccionados para evaluarlos personalmente.

## Descripción

El reclutador selecciona a los candidatos que han superado la fase inicial y programa la entrevista indicando fecha, hora y modalidad (virtual o presencial). El sistema envía invitaciones al candidato y al entrevistador, y registra la información de la entrevista en el perfil de la candidatura.

## Criterios de Aceptación

- **Dado** que el reclutador está en la pantalla de detalle de un candidato preseleccionado,  
  **cuando** programe la entrevista indicando fecha, hora y modalidad,  
  **entonces** el sistema creará el evento y enviará notificaciones (correo o SMS) tanto al candidato como al entrevistador.

- **Dado** que se haya programado una entrevista,  
  **cuando** falten 24 horas para la cita,  
  **entonces** el sistema enviará un recordatorio automático a ambas partes (si está configurado).

## Notas Adicionales

- Puede integrarse con calendarios externos (Google, Outlook) para sincronizar la cita.
- Se deben contemplar recordatorios automáticos (24h, 2h antes) y la posibilidad de reprogramar o cancelar.

## Tareas

- **Formulario de entrevista:** Diseñar la interfaz para introducir fecha, hora y modalidad.
- **Persistencia:** Guardar la información de la entrevista (Interview Entity) en la base de datos.
- **Notificaciones:** Integrar con el servicio de mensajería para enviar invitaciones y recordatorios.
- **Integración con calendarios (opcional):** Implementar la sincronización si se requiere.
- **Pruebas de usabilidad:** Verificar la claridad del flujo para el reclutador y el candidato.

---

# 3. Panel de Control con Métricas Básicas

## User Story

**Como Reclutador**, quiero ver un panel de control con métricas básicas (tiempo promedio de contratación, número de candidatos por oferta, etc.) para medir la eficiencia del proceso.

## Descripción

El sistema mostrará un dashboard con indicadores clave (KPI) que permitan al reclutador o al equipo de RRHH evaluar la efectividad de su proceso de selección, identificar cuellos de botella y tomar decisiones basadas en datos.

## Criterios de Aceptación

- **Dado** que el reclutador accede al panel de control,  
  **cuando** existan datos de ofertas y candidatos en el sistema,  
  **entonces** se mostrarán métricas como el tiempo promedio de contratación, el número de candidatos por oferta, la tasa de conversión, etc.

- **Dado** que el reclutador desee filtrar por rango de fechas,  
  **cuando** seleccione un período (por ejemplo, último trimestre),  
  **entonces** el sistema recalculará las métricas y actualizará la visualización.

## Notas Adicionales

- Se recomienda comenzar con KPIs sencillos y luego expandir a métricas más avanzadas (coste por contratación, satisfacción del candidato, etc.).
- El panel de control debe ser responsivo y fácil de entender (gráficos, tablas).

## Tareas

- **Definición de KPIs:** Identificar las métricas clave (tiempo promedio de contratación, número de postulaciones, etc.).
- **Consultas y cálculos:** Implementar la lógica de agregación de datos (SQL, ETL, etc.).
- **Diseño de dashboard:** Crear gráficos y tablas que muestren las métricas de forma clara.
- **Filtros:** Permitir filtrar por fechas, ofertas específicas, reclutadores, etc.
- **Validación de datos:** Asegurar la exactitud de los cálculos con datos de prueba y escenarios reales.



# ------------- BACKLOGS------------- ###


-Backlog Resultado Prompt elegido (3):



# Backlog Refinado (Subhistorias) con Priorización WSJF

A continuación, se **refinan** las tres User Stories principales (Filtrado de Candidatos, Programación de Entrevistas y Panel de Control con Métricas) en **subhistorias** más pequeñas y manejables. Para cada subhistoria se indica:

- **Criterio de Aceptación** (Dado/Cuando/Entonces)  
- **Valor de Negocio** (VB)  
- **Complejidad** (Esfuerzo estimado)  
- **WSJF Score** = (VB / Complejidad) o la versión simplificada de WSJF para historias cortas  
- **Prioridad** (según WSJF)

> **Nota**: La fórmula original de WSJF considera más factores (Urgencia, Reducción de Riesgo, etc.). Para simplificar, usamos un **WSJF aproximado** que relaciona **Valor de Negocio** con **Complejidad**.

---

## 1. Filtrado de Candidatos

### 1.1. Subhistoria: “Búsqueda por Palabra Clave”

- **Descripción**: Permitir al reclutador introducir una palabra o frase y mostrar candidatos cuyos CV o perfiles contengan dicha palabra.  
- **Criterio de Aceptación**  
  - **Dado** que el reclutador esté en la vista de “Candidatos”,  
  - **cuando** introduzca una palabra clave (p. ej. “Java”),  
  - **entonces** se listarán únicamente los candidatos que tengan “Java” en su CV, habilidades o descripción.  
- **Valor de Negocio (VB)**: 8  
- **Complejidad**: 3  
- **WSJF**: 8 / 3 ≈ 2.7  
- **Prioridad**: Alta (dentro del conjunto de subhistorias de Filtrado)

### 1.2. Subhistoria: “Filtro por Ubicación y Experiencia”

- **Descripción**: Añadir campos para filtrar por ubicación (ciudad/país) y años de experiencia.  
- **Criterio de Aceptación**  
  - **Dado** que el reclutador aplique filtros de “Ubicación = Madrid” y “Experiencia >= 3 años”,  
  - **cuando** confirme la búsqueda,  
  - **entonces** se mostrarán candidatos que cumplan ambas condiciones.  
- **Valor de Negocio (VB)**: 6  
- **Complejidad**: 3  
- **WSJF**: 6 / 3 = 2.0  
- **Prioridad**: Media

### 1.3. Subhistoria: “Paginación y Ordenamiento”

- **Descripción**: Implementar paginación y opción de ordenar candidatos por nombre, experiencia o fecha de postulación.  
- **Criterio de Aceptación**  
  - **Dado** que haya más de 50 candidatos,  
  - **cuando** el reclutador navegue a la siguiente página o cambie el criterio de orden,  
  - **entonces** el sistema responderá en menos de 2 segundos y mostrará la lista ordenada/paginada.  
- **Valor de Negocio (VB)**: 5  
- **Complejidad**: 4  
- **WSJF**: 5 / 4 = 1.25  
- **Prioridad**: Baja (pero importante para usabilidad)

---

## 2. Programación de Entrevistas

### 2.1. Subhistoria: “Creación de Entrevista (Fecha/Hora/Modalidad)”

- **Descripción**: El reclutador puede programar la entrevista indicando fecha, hora y si es virtual o presencial.  
- **Criterio de Aceptación**  
  - **Dado** que el reclutador seleccione un candidato preseleccionado,  
  - **cuando** introduzca fecha, hora y modalidad,  
  - **entonces** la entrevista se guardará en el sistema con estado “Scheduled”.  
- **Valor de Negocio (VB)**: 8  
- **Complejidad**: 3  
- **WSJF**: 8 / 3 ≈ 2.7  
- **Prioridad**: Alta

### 2.2. Subhistoria: “Notificaciones de Invitación”

- **Descripción**: Enviar un correo/SMS al candidato y al reclutador con los detalles de la entrevista.  
- **Criterio de Aceptación**  
  - **Dado** que se haya creado una entrevista con fecha/hora,  
  - **cuando** se confirme la programación,  
  - **entonces** el candidato y el reclutador recibirán un correo/SMS con la información de la cita.  
- **Valor de Negocio (VB)**: 7  
- **Complejidad**: 2  
- **WSJF**: 7 / 2 = 3.5  
- **Prioridad**: Muy Alta

### 2.3. Subhistoria: “Reprogramar o Cancelar Entrevista”

- **Descripción**: Permitir cambiar fecha/hora o cancelar la entrevista y notificar a las partes involucradas.  
- **Criterio de Aceptación**  
  - **Dado** que exista una entrevista en estado “Scheduled”,  
  - **cuando** el reclutador la reprograme o la cancele,  
  - **entonces** se actualizará el estado y se enviará la notificación correspondiente.  
- **Valor de Negocio (VB)**: 6  
- **Complejidad**: 3  
- **WSJF**: 6 / 3 = 2.0  
- **Prioridad**: Media

### 2.4. Subhistoria: “Recordatorio Automático (24h Antes)”

- **Descripción**: Enviar un recordatorio automático 24 horas antes de la entrevista si no se ha cancelado.  
- **Criterio de Aceptación**  
  - **Dado** que la entrevista siga en estado “Scheduled” y falten 24 horas para la cita,  
  - **cuando** se cumpla ese tiempo,  
  - **entonces** se disparará un correo/SMS de recordatorio al candidato y reclutador.  
- **Valor de Negocio (VB)**: 5  
- **Complejidad**: 3  
- **WSJF**: 5 / 3 ≈ 1.7  
- **Prioridad**: Baja

---

## 3. Panel de Control con Métricas

### 3.1. Subhistoria: “Cálculo de Tiempo Promedio de Contratación”

- **Descripción**: Mostrar la métrica “tiempo promedio de contratación” (desde la postulación hasta la contratación).  
- **Criterio de Aceptación**  
  - **Dado** que existan candidatos contratados,  
  - **cuando** el reclutador acceda al panel,  
  - **entonces** se mostrará la cifra del promedio de días desde la postulación hasta la contratación.  
- **Valor de Negocio (VB)**: 6  
- **Complejidad**: 4  
- **WSJF**: 6 / 4 = 1.5  
- **Prioridad**: Media

### 3.2. Subhistoria: “Número de Candidatos por Oferta”

- **Descripción**: Graficar cuántos candidatos ha recibido cada oferta.  
- **Criterio de Aceptación**  
  - **Dado** que existan varias ofertas con candidaturas,  
  - **cuando** el reclutador entre al panel de métricas,  
  - **entonces** se mostrará un gráfico de barras con el número de candidatos por oferta.  
- **Valor de Negocio (VB)**: 5  
- **Complejidad**: 3  
- **WSJF**: 5 / 3 ≈ 1.7  
- **Prioridad**: Baja

### 3.3. Subhistoria: “Filtro de Fechas en el Panel”

- **Descripción**: Permitir seleccionar un rango de fechas para recalcular las métricas de contrataciones, candidaturas, etc.  
- **Criterio de Aceptación**  
  - **Dado** que el reclutador seleccione un rango de fechas (ej. último trimestre),  
  - **cuando** se aplique el filtro,  
  - **entonces** el panel se actualizará mostrando únicamente los datos dentro de ese rango.  
- **Valor de Negocio (VB)**: 4  
- **Complejidad**: 3  
- **WSJF**: 4 / 3 ≈ 1.3  
- **Prioridad**: Baja

---

## Resumen de Prioridades por Subhistorias (WSJF)

A modo de ejemplo, se listan las subhistorias con su WSJF aproximado y prioridad (de mayor a menor):

| **Subhistoria**                                     | **WSJF** | **Prioridad** |
|-----------------------------------------------------|:-------:|:------------:|
| **2.2. Notificaciones de Invitación**               | 3.5     | Muy Alta     |
| **2.1. Creación de Entrevista (Fecha/Hora/Modalidad)** | 2.7     | Alta         |
| **1.1. Búsqueda por Palabra Clave**                 | 2.7     | Alta         |
| **2.3. Reprogramar o Cancelar Entrevista**          | 2.0     | Media        |
| **1.2. Filtro por Ubicación y Experiencia**         | 2.0     | Media        |
| **3.1. Cálculo de Tiempo Promedio de Contratación** | 1.5     | Media        |
| **2.4. Recordatorio Automático (24h Antes)**        | 1.7     | Baja         |
| **3.2. Número de Candidatos por Oferta**            | 1.7     | Baja         |
| **1.3. Paginación y Ordenamiento**                  | 1.25    | Baja         |
| **3.3. Filtro de Fechas en el Panel**               | 1.3     | Baja         |

> **Nota**: Se observa que la **creación y notificación de entrevistas** y el **filtro por palabra clave** son las subhistorias de mayor valor relativo respecto a su complejidad. Las funciones de **métricas** y **filtros adicionales** tienen un menor WSJF, por lo que podrían abordarse después de las más prioritarias.

---

## Conclusión

Este **backlog refinado** divide las User Stories principales en **subhistorias** concretas, asignando un **valor de negocio** y una **complejidad** estimada para calcular un **WSJF** aproximado. De esta forma, el equipo puede **planificar** y **desarrollar** funcionalidades de manera incremental, atacando primero las que aportan **mayor valor** con menor **esfuerzo**.  


# ------------ TICKETS DE TRABAJO ------------ ###



# Sprint Backlog: Programación de Entrevistas

A continuación, se detallan los **tickets de trabajo** necesarios para implementar la User Story **“Programación de Entrevistas”**. Cada ticket se ha estructurado según los elementos solicitados: Título, Descripción, Criterios de Aceptación, Prioridad, Estimación de Esfuerzo, Asignación, Etiquetas, Comentarios/Notas, Enlaces/Referencias e Historial de Cambios.

---

## Ticket 1: Diseñar y Crear la Entidad "Interview" en la Base de Datos

1. **Título**  
   - Diseñar y Crear la Entidad "Interview" en la Base de Datos

2. **Descripción**  
   - **Propósito**: Definir la estructura necesaria para almacenar información de entrevistas (fecha, hora, modalidad, estado, feedback, etc.).  
   - **Detalles Específicos**:  
     - Crear tabla/colección `Interview` con los campos: `id`, `application_id`, `scheduled_date`, `modality` (virtual/presencial), `status` (Scheduled, Completed, Canceled, etc.), `feedback`, `interviewer_id`.  
     - Establecer relación con la entidad `Application` (FK o referencia).

3. **Criterios de Aceptación**  
   - **Dado** que se ejecute la migración o script de creación,  
   - **cuando** el entorno de desarrollo se inicie,  
   - **entonces** la tabla/colección `Interview` existirá y será accesible para CRUD básico.

4. **Prioridad**  
   - Alta (bloquea la creación y programación de entrevistas).

5. **Estimación de Esfuerzo**  
   - 3 puntos de historia.

6. **Asignación**  
   - Equipo Backend (Desarrollador/a 1).

7. **Etiquetas**  
   - `#backend`, `#database`, `#high-priority`, `#programacion-entrevistas`.

8. **Comentarios / Notas**  
   - Se recomienda agregar índices en `application_id` para facilitar búsquedas y joins.  
   - Verificar si se necesitará un campo para `calendar_event_id` en caso de integración con calendarios externos.

9. **Enlaces / Referencias**  
   - [Diseño Entidad Interview (Especificación)](#)  
   - [Modelo de Datos del ATS](#)

10. **Historial de Cambios**  
   - *09/09/2025*: Creado el ticket.  
   - *10/09/2025*: Agregado campo `modality` tras revisión de requisitos.

---

## Ticket 2: Endpoint para Crear y Guardar Entrevistas

1. **Título**  
   - Endpoint para Crear y Guardar Entrevistas

2. **Descripción**  
   - **Propósito**: Permitir la programación de entrevistas desde la aplicación, recibiendo datos (fecha/hora, modalidad, entrevistador).  
   - **Detalles Específicos**:  
     - Crear endpoint `POST /interviews` con validaciones.  
     - Asegurar que `application_id` exista y que el estado de la candidatura permita la programación de entrevistas.

3. **Criterios de Aceptación**  
   - **Dado** que el reclutador envíe una solicitud `POST /interviews` con datos válidos,  
   - **cuando** el servidor reciba la petición,  
   - **entonces** se creará un registro en la tabla `Interview` con estado “Scheduled” y se devolverá un `201 Created`.

4. **Prioridad**  
   - Alta (funcionalidad principal de la programación).

5. **Estimación de Esfuerzo**  
   - 5 puntos de historia.

6. **Asignación**  
   - Equipo Backend (Desarrollador/a 2).

7. **Etiquetas**  
   - `#backend`, `#api`, `#programacion-entrevistas`, `#high-priority`.

8. **Comentarios / Notas**  
   - Validar campos obligatorios (`scheduled_date`, `application_id`, `modality`).  
   - Manejar errores de negocio (p.ej., si `application_id` no existe o el candidato está en estado no apto para entrevistas).

9. **Enlaces / Referencias**  
   - [Entidad Interview creada en Ticket 1](#)  
   - [Casos de Uso - Programación de Entrevistas](#)

10. **Historial de Cambios**  
   - *09/09/2025*: Creado el ticket.  
   - *11/09/2025*: Se actualiza para incluir validación de `modality`.

---

## Ticket 3: UI para Programar Entrevistas (Front-End)

1. **Título**  
   - UI para Programar Entrevistas (Front-End)

2. **Descripción**  
   - **Propósito**: Proporcionar al reclutador una pantalla/formulario donde definir la entrevista (fecha, hora, modalidad).  
   - **Detalles Específicos**:  
     - Formulario con selector de fecha/hora (DatePicker).  
     - Opción para elegir modalidad (virtual/presencial).  
     - Botón “Programar Entrevista” que envíe la información al endpoint correspondiente.

3. **Criterios de Aceptación**  
   - **Dado** que el reclutador está en la vista del candidato,  
   - **cuando** haga clic en “Programar Entrevista” y complete los datos,  
   - **entonces** se llamará al endpoint `POST /interviews` y, si es exitoso, se mostrará un mensaje de confirmación.

4. **Prioridad**  
   - Media (necesario para la experiencia del reclutador, pero depende del endpoint ya creado).

5. **Estimación de Esfuerzo**  
   - 3 puntos de historia.

6. **Asignación**  
   - Equipo Front-End (Desarrollador/a 3).

7. **Etiquetas**  
   - `#frontend`, `#ui`, `#programacion-entrevistas`, `#medium-priority`.

8. **Comentarios / Notas**  
   - Se debe manejar feedback de errores (p.ej., fecha no válida, `application_id` inexistente).  
   - Considerar responsive design y usabilidad.

9. **Enlaces / Referencias**  
   - [Endpoint POST /interviews (Ticket 2)](#)  
   - [Diseño de la pantalla de Candidatos (Mockups)](#)

10. **Historial de Cambios**  
   - *09/09/2025*: Creado el ticket.  
   - *12/09/2025*: Añadida validación de calendario.

---

## Ticket 4: Envío de Notificaciones de Invitación

1. **Título**  
   - Envío de Notificaciones de Invitación

2. **Descripción**  
   - **Propósito**: Notificar a candidato y reclutador/entrevistador cuando se crea una nueva entrevista.  
   - **Detalles Específicos**:  
     - Integrar con servicio de mensajería (email/SMS).  
     - Generar plantilla de correo con fecha/hora y enlace (si es virtual).  
     - Actualizar la lógica de `POST /interviews` para disparar el envío.

3. **Criterios de Aceptación**  
   - **Dado** que el reclutador programa una entrevista con datos válidos,  
   - **cuando** se guarde en la base de datos,  
   - **entonces** el sistema enviará un correo/SMS al candidato y al entrevistador con la información de la entrevista.

4. **Prioridad**  
   - Alta (refuerza la comunicación y usabilidad).

5. **Estimación de Esfuerzo**  
   - 4 puntos de historia.

6. **Asignación**  
   - Equipo Backend (Desarrollador/a 2) con soporte de Infraestructura.

7. **Etiquetas**  
   - `#backend`, `#notificaciones`, `#programacion-entrevistas`, `#infra`.

8. **Comentarios / Notas**  
   - Verificar credenciales y limitaciones del servicio de correo/SMS.  
   - Manejar reintentos si falla el envío.

9. **Enlaces / Referencias**  
   - [Servicio de Mensajería (SendGrid, Twilio, etc.)](#)  
   - [Endpoint POST /interviews (Ticket 2)](#)

10. **Historial de Cambios**  
   - *09/09/2025*: Creado el ticket.  
   - *12/09/2025*: Se incluye la integración con SMS.

---

## Ticket 5: Reprogramar/Cancelar Entrevista

1. **Título**  
   - Reprogramar/Cancelar Entrevista

2. **Descripción**  
   - **Propósito**: Permitir cambiar fecha/hora de una entrevista ya programada o cancelarla. Notificar a los involucrados del cambio.  
   - **Detalles Específicos**:  
     - Endpoint `PUT /interviews/{id}` para actualizar fecha/hora o estado.  
     - Enviar notificaciones de actualización o cancelación.

3. **Criterios de Aceptación**  
   - **Dado** que exista una entrevista en estado “Scheduled”,  
   - **cuando** el reclutador la reprograma o la cancela,  
   - **entonces** se actualiza en la base de datos y se dispara una notificación con la nueva información o aviso de cancelación.

4. **Prioridad**  
   - Media (importante para la flexibilidad de la agenda).

5. **Estimación de Esfuerzo**  
   - 4 puntos de historia.

6. **Asignación**  
   - Equipo Backend (Desarrollador/a 2) y Front-End (Desarrollador/a 3) para la UI.

7. **Etiquetas**  
   - `#backend`, `#frontend`, `#programacion-entrevistas`, `#medium-priority`.

8. **Comentarios / Notas**  
   - Asegurar que el estado cambie a “Canceled” o que la fecha/hora se actualice correctamente.  
   - En caso de cancelación, eliminar la cita de calendario externo (si está integrado).

9. **Enlaces / Referencias**  
   - [API PUT /interviews (Diseño)](#)  
   - [Ticket 4 - Notificaciones de Invitación](#)

10. **Historial de Cambios**  
   - *09/09/2025*: Creado el ticket.  
   - *12/09/2025*: Se añade la lógica para eliminar evento del calendario externo.

---

## Ticket 6: Recordatorio Automático (24h Antes)

1. **Título**  
   - Recordatorio Automático (24h Antes)

2. **Descripción**  
   - **Propósito**: Enviar un recordatorio a candidatos y entrevistadores 24 horas antes de la entrevista, siempre que no se haya cancelado.  
   - **Detalles Específicos**:  
     - Crear un job o servicio programado que revise las entrevistas en estado “Scheduled” y calcule el tiempo restante.  
     - Enviar notificación si faltan 24h.

3. **Criterios de Aceptación**  
   - **Dado** que una entrevista esté en “Scheduled” con fecha/hora futura,  
   - **cuando** falten exactamente 24 horas,  
   - **entonces** se enviará un correo/SMS de recordatorio a candidato y entrevistador.

4. **Prioridad**  
   - Baja (mejora la experiencia, pero no bloquea la funcionalidad básica).

5. **Estimación de Esfuerzo**  
   - 3 puntos de historia.

6. **Asignación**  
   - Equipo Backend (Desarrollador/a 1 o 2).

7. **Etiquetas**  
   - `#backend`, `#infra`, `#programacion-entrevistas`, `#low-priority`.

8. **Comentarios / Notas**  
   - Se recomienda un cron job o un servicio que corra cada hora y verifique las entrevistas pendientes.  
   - Ajustar la zona horaria si es relevante para usuarios en diferentes lugares.

9. **Enlaces / Referencias**  
   - [Servicio de Mensajería (Ticket 4)](#)  
   - [Diseño Cron Job / Scheduling en la Infraestructura](#)

10. **Historial de Cambios**  
   - *09/09/2025*: Creado el ticket.  
   - *13/09/2025*: Añadido soporte multi-zona horaria.

---

## Resumen de Tickets

| **Ticket**                                                  | **Prioridad** | **Estimación** | **Responsables**                |
|-------------------------------------------------------------|--------------:|---------------:|---------------------------------|
| **1. Diseñar Entidad "Interview"**                          | Alta          | 3 pts          | Backend (Dev 1)                 |
| **2. Endpoint para Crear Entrevistas**                      | Alta          | 5 pts          | Backend (Dev 2)                 |
| **3. UI para Programar Entrevistas**                        | Media         | 3 pts          | Front-End (Dev 3)               |
| **4. Envío de Notificaciones de Invitación**                | Alta          | 4 pts          | Backend (Dev 2), Infra          |
| **5. Reprogramar/Cancelar Entrevista**                      | Media         | 4 pts          | Backend (Dev 2), Front-End (Dev 3) |
| **6. Recordatorio Automático (24h Antes)**                  | Baja          | 3 pts          | Backend (Dev 1 o 2)             |

Este **Sprint Backlog** aborda todas las subtareas técnicas necesarias para completar la funcionalidad de **Programación de Entrevistas**, siguiendo el **formato** de tickets propuesto y cubriendo la **información esencial** para que el equipo comprenda y ejecute cada tarea.



# ------------ ESTIMACIÓN ESFUERZO ------------ ###



# Estimación de Esfuerzo (Planning Poker) – Sprint Backlog: Programación de Entrevistas

A continuación, se presenta la **estimación de los tickets** del Sprint Backlog utilizando la metodología de **Planning Poker** y **Puntos de Historia**. Se incluyen las **votaciones** de cada integrante del equipo (a modo de ejemplo) y el **consenso final** alcanzado para cada ticket.

---

## Equipo de Desarrollo (Ejemplo)

- **Dev1** (Backend)  
- **Dev2** (Backend / Infra)  
- **Dev3** (Front-End)  
- **QA1** (Testing / Calidad)

> **Nota**: El número resultante de puntos de historia es el **consenso** tras la discusión y la votación.

---

## 1. Diseñar Entidad "Interview" en la Base de Datos

| **Integrante** | **Votación** |
|:--------------:|:-----------:|
| **Dev1**       | 3           |
| **Dev2**       | 5           |
| **Dev3**       | 3           |
| **QA1**        | 3           |
| **Consenso**   | **3**       |

**Razonamiento**:  
- Dev2 considera que podrían surgir complicaciones en la migración.  
- El resto opina que es relativamente straightforward.  
- Se discute y se decide en **3 puntos** porque el riesgo adicional que percibe Dev2 se mitiga con la experiencia del equipo en migraciones.

---

## 2. Endpoint para Crear y Guardar Entrevistas

| **Integrante** | **Votación** |
|:--------------:|:-----------:|
| **Dev1**       | 5           |
| **Dev2**       | 5           |
| **Dev3**       | 3           |
| **QA1**        | 5           |
| **Consenso**   | **5**       |

**Razonamiento**:  
- Dev3 opina que no requiere demasiada lógica compleja en front-end, pero para el back-end se debe validar `application_id`, manejar errores y notificaciones.  
- QA1 considera que habrá bastantes casos de prueba.  
- Se llega a un **consenso** en **5 puntos**.

---

## 3. UI para Programar Entrevistas (Front-End)

| **Integrante** | **Votación** |
|:--------------:|:-----------:|
| **Dev1**       | 2           |
| **Dev2**       | 3           |
| **Dev3**       | 3           |
| **QA1**        | 3           |
| **Consenso**   | **3**       |

**Razonamiento**:  
- Dev1, que es principalmente back-end, ve esto más sencillo (no percibe riesgos).  
- Dev2 y Dev3 coinciden en que el front-end necesitará validaciones, manejo de errores, etc.  
- QA1 estima un testing moderado.  
- Se acuerda **3 puntos** como consenso.

---

## 4. Envío de Notificaciones de Invitación

| **Integrante** | **Votación** |
|:--------------:|:-----------:|
| **Dev1**       | 5           |
| **Dev2**       | 3           |
| **Dev3**       | 5           |
| **QA1**        | 5           |
| **Consenso**   | **4** (Aprox.) |

**Razonamiento**:  
- Algunos ven mayor complejidad por la integración con un servicio externo (SendGrid, Twilio, etc.).  
- Dev2, con experiencia en infra, lo ve algo más simple.  
- Tras la discusión, se acuerda un **término medio** de **4 puntos**.

---

## 5. Reprogramar/Cancelar Entrevista

| **Integrante** | **Votación** |
|:--------------:|:-----------:|
| **Dev1**       | 5           |
| **Dev2**       | 5           |
| **Dev3**       | 3           |
| **QA1**        | 5           |
| **Consenso**   | **5**       |

**Razonamiento**:  
- Se deben manejar estados, notificaciones de cambios, posibles conflictos con calendarios.  
- El front-end requiere un UI adicional para reprogramar/cancelar.  
- QA1 percibe múltiples escenarios de prueba (cambio de fecha, cancelación, verificación de notificaciones).  
- Se decide en **5 puntos**.

---

## 6. Recordatorio Automático (24h Antes)

| **Integrante** | **Votación** |
|:--------------:|:-----------:|
| **Dev1**       | 3           |
| **Dev2**       | 3           |
| **Dev3**       | 2           |
| **QA1**        | 3           |
| **Consenso**   | **3**       |

**Razonamiento**:  
- Se necesita un **job programado** o un servicio que verifique entrevistas pendientes y envíe notificaciones.  
- Dev3 (front-end) estima menor complejidad, ya que no es muy UI-intensivo.  
- Dev1, Dev2 y QA1 coinciden en que hay que tener cuidado con la zona horaria y reintentos.  
- Se cierra en **3 puntos**.

---

## Resumen Final de Estimaciones

| **Ticket**                                                | **Consenso** (Puntos) |
|-----------------------------------------------------------|:---------------------:|
| **1. Diseñar Entidad "Interview"**                        | 3                     |
| **2. Endpoint para Crear Entrevistas**                    | 5                     |
| **3. UI para Programar Entrevistas**                      | 3                     |
| **4. Envío de Notificaciones de Invitación**              | 4                     |
| **5. Reprogramar/Cancelar Entrevista**                    | 5                     |
| **6. Recordatorio Automático (24h Antes)**                | 3                     |

**Total de Puntos de Historia** para la **User Story Programación de Entrevistas** en este sprint: **3 + 5 + 3 + 4 + 5 + 3 = 23 puntos**.

---

## Conclusión

Este cuadro de **votaciones** y el **consenso final** reflejan cómo el equipo ha **discutido** y **estimado** el esfuerzo requerido para cada ticket de trabajo relacionado con la Programación de Entrevistas, usando la metodología **Planning Poker** y **Story Points**. Se obtiene así una visión clara de la **complejidad** relativa de cada parte del trabajo y una **base** para la planificación del sprint.  
