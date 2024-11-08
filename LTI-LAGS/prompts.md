
❗Se toma como contexto  el chat compartido por Dago y desde este se comienza las iteraciones con los diferentes prompts

Modelo 👉 CHATGPT-4o

## **Prompt para generar User Stories para un ATS**

> Como Product Manager y Business Analyst, tu misión es preparar las **User Stories** para la implementación de un sistema ATS. Usando la información del PRD básico y los documentos de backlog, funcionalidades clave, casos de uso y modelo de datos, sigue estos pasos:
> 
> ### Instrucciones:
> 
> 1. **Contexto**:
>    Este sistema ATS busca optimizar el proceso de reclutamiento mediante características como la automatización de tareas, colaboración en tiempo real entre reclutadores y managers, IA avanzada para el emparejamiento de candidatos, y una experiencia personalizada para los candidatos.
> 
> 2. **Estructura de User Stories**:
>    Utiliza el formato estándar de User Stories:
>    
>    ```
>    Como [tipo de usuario], quiero [realizar una acción] para [obtener un beneficio].
>    ```
> 
> 3. **Criterios de Aceptación**:
>    Cada User Story debe contener criterios de aceptación claros, siguiendo el formato:
>    
>    ```
>    Dado que [contexto inicial], cuando [acción realizada], entonces [resultado esperado].
>    ```
> 
> 4. **Mínimo de User Stories**:
>    Redacta un mínimo de seis User Stories que abarquen las funcionalidades principales y los diferentes tipos de usuarios del sistema (reclutadores, managers de contratación, candidatos).
> 
> 5. **Ejemplo de Plantilla**:
>    Asegúrate de incluir los siguientes elementos en cada User Story:
>    - **Título**: Resumido y descriptivo
>    - **Descripción**: Descripción breve de la funcionalidad
>    - **Criterios de Aceptación**: Detalles específicos de funcionalidad
>    - **Notas Adicionales**: Información relevante para el desarrollo de la historia
>    - **Tareas**: Lista de tareas y subtareas necesarias para completar la historia
> 
> 6. **Ejemplo de User Story**:
>    
>    ```markdown
>    **Título de la Historia de Usuario**: Asignación Automática de Candidatos
>   
>    **Descripción**: Como reclutador, quiero que el sistema realice una asignación automática de los candidatos a vacantes relevantes, basada en sus habilidades y experiencia, para optimizar el proceso de preselección.
>   
>    **Criterios de Aceptación**:
>    - Dado que el candidato ha completado su perfil, cuando el sistema encuentra una vacante que coincide con sus habilidades, entonces asigna automáticamente al candidato a esa vacante.
>    - Dado que un candidato es asignado automáticamente a una vacante, cuando el reclutador revisa la lista de candidatos asignados, entonces puede ver al candidato en la vacante correspondiente.
>   
>    **Notas Adicionales**:
>    - La asignación debe realizarse en tiempo real y permitir personalización en los criterios de búsqueda.
>   
>    **Tareas**:
>    - Integrar API de matching de candidatos con vacantes
>    - Configurar alertas para notificaciones de asignación automática
>    - Pruebas de integración y validación de datos
>    ```
> 
> 7. **Consideraciones para la IA**:
>    Incorpora funcionalidades que utilicen IA para mejorar la experiencia, tales como la automatización en la preselección de candidatos y sugerencias en tiempo real.
> 
> 8. **Feedback del Equipo**:
>    Redacta las historias de usuario de manera colaborativa con el equipo de desarrollo y asegúrate de incluir criterios de aceptación para facilitar la validación de las funcionalidades.
> 
> ---
> 
> **Ejemplo de User Stories para el ATS:**
> 
> 1. **Asignación Automática de Candidatos a Vacantes**
> 2. **Panel de Colaboración en Tiempo Real para Reclutadores y Managers**
> 3. **Portal Personalizado para Seguimiento del Progreso del Candidato**
> 4. **Automatización de Programación de Entrevistas con IA**
> 5. **Evaluación Predictiva de Talento con Algoritmos de IA**
> 6. **Notificaciones Personalizadas de Progreso para Candidatos**
> 
> Cada historia debe alinearse con los objetivos de valor y optimización del sistema ATS, considerando los distintos roles de usuario y priorizando la experiencia del usuario final.

## **Prompt para generar Backlog de Producto

> 👎 Cuando envié este prompt no me dio buenos resultados se perdió su respuesta no fue coherente:
> 👉 Genera un Backlog de Producto para el sistema ATS con base en las User Stories definidas.

> 👍 Este prompt me dio mejores resultados cuando le adjunte las User Stories y le proporcione la documentación del modulo:
> 👉 Genera un Backlog de Producto priorizado para el sistema ATS usando las User Stories proporcionadas, aplicando la metodología RICE (Reach, Impact, Confidence, Effort). Para cada historia de usuario, calcula un puntaje de prioridad RICE considerando los siguientes factores: Alcance (Reach), Impacto (Impact), Confianza (Confidence), y Esfuerzo (Effort). Prioriza las historias en función del puntaje RICE, e incluye el título de la historia, descripción, tareas y criterios de aceptación en cada entrada del backlog.
> **Consideraciones:** 
> -Dame las respuesta en español
> -Genérame una tabla en mardown donde se visualicen los resultados

## **Prompt para generar  Tickets de trabajo

>Actúa como un equipo de desarrollo responsable de desglosar la User Story "Portal Personalizado para Seguimiento del Progreso del Candidato" en tickets de trabajo detallados. Organiza los tickets para abarcar todas las tareas necesarias, agrupándolos en etapas de implementación incremental para cubrir tanto el desarrollo de la interfaz como las funcionalidades internas del portal.
>
> Genera cada ticket de trabajo con los siguientes **componentes** mínimos para asegurar claridad y efectividad en la ejecución:
>
> 1. **Título Claro y Conciso**: Proporciona un título breve que capture el objetivo del ticket (por ejemplo, "Diseño de la interfaz del portal de candidatos").
> 
> 2. **Descripción Detallada**:
>    - **Propósito**: Describe brevemente por qué es necesario este ticket y qué problema o necesidad específica aborda dentro del contexto de la User Story.
>    - **Detalles Específicos**: Explica los requisitos específicos, restricciones o condiciones necesarias para la ejecución de la tarea. Incluye aspectos como el tipo de tecnología, integraciones necesarias o configuraciones técnicas.
> 
> 3. **Criterios de Aceptación**:
>    - Enumera claramente las condiciones que deben cumplirse para que el ticket sea considerado completo.
>    - Incluye pruebas de validación específicas, como validaciones de interfaz, pruebas de rendimiento y comportamiento esperado para los usuarios.
>
> 4. **Prioridad**:
>    - Asigna una prioridad basada en la urgencia de implementación y su impacto en la funcionalidad general del portal. Usa una escala de prioridad (Alta, Media, Baja) para cada ticket en función de su importancia en el flujo de trabajo.
>
> 5. **Estimación de Esfuerzo**:
>    - Proporciona una estimación de esfuerzo en puntos de historia o tiempo estimado, evaluando el trabajo necesario para completar cada ticket de acuerdo con su complejidad.
>
> 6. **Asignación**:
>    - Indica el rol o equipo responsable de completar el ticket (por ejemplo, equipo de Frontend, Backend, Integración).
>
> 7. **Etiquetas o Tags**:
>    - Añade etiquetas que clasifiquen el ticket según su tipo (UI, Backend, Seguridad, Integración), módulo relacionado, o sprint en el que se planea completar.
>
> 8. **Comentarios y Notas**:
>    - Incluye un espacio para comentarios y notas adicionales donde el equipo pueda agregar información relevante, hacer preguntas o actualizar el progreso del ticket.
>
> 9. **Enlaces o Referencias**:
>    - Agrega enlaces a documentos relacionados, diseños de interfaz, especificaciones o tickets anteriores que proporcionen contexto adicional y permitan una ejecución más completa del ticket.
>
> 10. **Historial de Cambios**:
>    - Documenta cualquier cambio importante en el ticket, como actualizaciones en la descripción, cambios de prioridad o modificaciones en los criterios de aceptación, asegurando un seguimiento de su evolución.
>   
---

**Instrucciones adicionales para el equipo de desarrollo**:
> 1. Organiza los tickets de forma que cada grupo cubra un objetivo específico del portal, como **desarrollo de interfaz de usuario (UI)**, **configuración de notificaciones automáticas**, e **integración con sistemas externos para escalabilidad y actualización en tiempo real**.
> 
> 2. Si algún ticket se relaciona con una User Story distinta o depende de otro ticket para completarse, especifica la dependencia y asigna el ticket a la historia de usuario correspondiente.
> 
> 3. Asegúrate de que el desarrollo de la interfaz y las notificaciones sean priorizados para cumplir con los criterios de aceptación de la User Story original, y organiza las tareas técnicas de backend e integración para etapas finales, de modo que garanticen un rendimiento óptimo y escalabilidad del sistema a largo plazo.

## **Prompt para generar  Estimación el esfuerzo de los Tickets

Actúa como facilitador de una sesión de estimación de esfuerzo para el equipo de desarrollo, utilizando la metodología **Planning Poker** para llegar a un consenso sobre el tiempo estimado en **horas** para cada uno de los tickets de trabajo. Sigue estos pasos para realizar la estimación de manera efectiva:
> 
> **Instrucciones Generales para la Estimación:**
> - **Contexto**: Lee en detalle cada uno de los tickets de trabajo del "Portal Personalizado para Seguimiento del Progreso del Candidato". Asegúrate de que todos los miembros del equipo comprendan bien los requisitos, criterios de aceptación, y detalles específicos de cada ticket antes de iniciar la estimación.
> - **Uso de Planning Poker (fpoker)**: Utiliza la metodología Planning Poker para que cada miembro del equipo proponga una estimación en horas para cada ticket de manera anónima. Esto fomentará una discusión abierta y permitirá llegar a un consenso.
> - **Discusión de Estimaciones**: Si las estimaciones varían significativamente entre los miembros del equipo, abre una discusión para explorar las razones de las diferencias en la estimación. Enfócate en identificar posibles áreas de complejidad o puntos que puedan requerir aclaración.
> 
> **Componentes Específicos para cada Ticket de Trabajo:**
> 1. **Ticket 1: Diseño de la Interfaz del Portal de Candidatos**
>    - **Discusión Clave**: Revisen la complejidad de diseñar una interfaz intuitiva y responsiva. Consideren también el tiempo necesario para asegurar que cumpla con las pautas de diseño de la empresa.
>    - **Estimación Final en Horas**: Definan una estimación de esfuerzo en horas para completar el diseño inicial y ajustar cualquier detalle visual tras la revisión.
>
> 2. **Ticket 2: Implementación de la Interfaz en Frontend**
>    - **Discusión Clave**: Analicen el esfuerzo de traducir el diseño en una implementación funcional y responsiva, considerando también la carga de trabajo de integración en tiempo real con el backend.
>    - **Estimación Final en Horas**: Asignen horas para el trabajo de desarrollo y pruebas para asegurar que el diseño se despliegue correctamente en dispositivos móviles y de escritorio.
>
> 3. **Ticket 3: Configuración de Notificaciones en Tiempo Real**
>    - **Discusión Clave**: Estimen el esfuerzo necesario para integrar el sistema de notificaciones en tiempo real, teniendo en cuenta la complejidad de personalización y los sistemas de mensajería.
>    - **Estimación Final en Horas**: Consensúen una estimación para cubrir la implementación y pruebas de esta funcionalidad.
>
> 4. **Ticket 4: Configuración de Preferencias de Notificación en la Interfaz**
>    - **Discusión Clave**: Consideren el esfuerzo de añadir opciones de configuración en la interfaz y de asegurar que se sincronice con el backend para persistencia.
>    - **Estimación Final en Horas**: Lleguen a un acuerdo sobre las horas necesarias para el desarrollo y prueba de las opciones de configuración.
>
> 5. **Ticket 5: Integración de Actualización en Tiempo Real con Backend**
>    - **Discusión Clave**: Evalúen la complejidad de la comunicación en tiempo real entre frontend y backend, considerando el uso de tecnologías como WebSocket.
>    - **Estimación Final en Horas**: Acuerden una estimación en horas para la implementación y las pruebas de estabilidad de la integración.
>
> 6. **Ticket 6: Persistencia y Almacenamiento de Preferencias de Notificación**
>    - **Discusión Clave**: Analicen los requisitos para almacenar y gestionar las preferencias de notificación en la base de datos de manera segura.
>    - **Estimación Final en Horas**: Determinen el tiempo necesario para el desarrollo, pruebas y validación de la persistencia.
>
> 7. **Ticket 7: Pruebas de Funcionalidad del Portal**
>    - **Discusión Clave**: Estimen el esfuerzo para realizar pruebas exhaustivas de cada funcionalidad, incluyendo notificaciones y actualización en tiempo real.
>    - **Estimación Final en Horas**: Acordar una estimación de horas para cubrir las pruebas y correcciones.
>
> 8. **Ticket 8: Pruebas de Rendimiento y Escalabilidad**
>    - **Discusión Clave**: Consideren el tiempo necesario para realizar pruebas de rendimiento, especialmente bajo cargas altas.
>    - **Estimación Final en Horas**: Lleven a consenso una estimación para las pruebas de rendimiento, considerando pruebas de estrés y ajuste de escalabilidad.
>
>  **Documentación de Resultados:**
> - **Registro de Estimaciones**: Documenta la estimación final en horas para cada ticket, incluyendo cualquier comentario relevante de la discusión.
> - **Historial de Estimaciones**: Mantén un historial de los cambios en estimaciones para cada ticket, en caso de que sea necesario ajustar las horas en el futuro.
> - **Notificación de Dependencias**: Si alguna estimación depende de otros tickets o requiere ajustes adicionales, documenta esta relación para asegurar la alineación en futuras estimaciones.


