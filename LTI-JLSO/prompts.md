| IA Agent: | Chat GPT |
| --- | --- |
| Modelo: | GPT-4o |
| Autor: | Jorge Luis Sánchez Ocampo |

Este documento contiene los prompts utilizados para crear el Product Backlog del proyecto ATS(Applicant Tracking System), para la empresa LTI. Ejercicio del curso AI4devs.

## Contexto

1. PRD - Se crea un prompt para validar el contenido del documento(resultado del ejercicio anterior, en la sección de diseño) que se va a pasar como contexto:
    1. Prompt
        
            Explícame brevemente el contenido de el siguiente documento adjunto
        
    2. Respuesta

            El documento describe el diseño de un sistema de gestión de candidatos (ATS, por sus siglas en inglés) para la empresa LTI, una plataforma destinada a optimizar los procesos de selección de personal. Incluye:

            1.	Descripción del software: Expone el valor añadido y ventajas competitivas del ATS, como la automatización de tareas, la mejora de la experiencia del usuario, análisis predictivo, integración con otros sistemas y personalización.
            2.	Casos de uso: Presenta tres casos principales con sus respectivos diagramas:
            •	Publicación de vacantes.
            •	Aplicación a vacantes por parte de candidatos.
            •	Revisión y clasificación de candidatos por reclutadores.
            3.	Modelo de datos: Define las entidades principales del sistema, sus atributos y relaciones (como reclutador, vacante, candidato, aplicación y plataforma de publicación).
            4.	Arquitectura de alto nivel: Describe una arquitectura basada en microservicios para gestionar usuarios, vacantes, aplicaciones, análisis y notificaciones, junto con un diagrama de contenedores y explicaciones detalladas.
            5.	Diagramas C4: Incluye diagramas de contexto, contenedores y componentes para mostrar la interacción entre los elementos del sistema y con servicios externos, como proveedores de autenticación.

            Este diseño tiene como objetivo hacer el sistema escalable, eficiente y fácil de integrar, con un enfoque modular en microservicios para simplificar su mantenimiento y evolución.
        
2. Product Backlog - Contexto sobre las tareas que debemos realizar
    1. Prompt
        
        ```markdown
        Utiliza el documento del anterior prompt como base de conocimiento para las siguientes tareas, son 4 tareas en total y vamos a ir resolviéndolas una a una, a medida que te vaya indicando. Esta información solamente es para que tengas el contexto inicial de las tareas a realizar: 
        
        En este ejercicio vas a actuar como un Product Manager y Business Analyst. 
        
        Usando los documentos que generaste en la sección anterior y que conforman un PRD básico (funcionalidades clave, casos de uso, modelo de datos...)(DOCUMENTO PROPORCIONADO EN EL PROMPT ANTERIOR), tu misión es preparar la documentación necesaria para empezar a implementar LTI:
        
        1. Generar las User Stories. Puedes implementar tantas como quieras y puedas, el mínimo son 2.
        
        2. Arma el Backlog de producto con las User Stories, priorizándolas como consideres conveniente acorde a alguna metodología concreta.
        
        3. Elige la User Story que prefieras, y genera los Tickets de trabajo. Aterrízalos técnicamente, tal y como se hace en las reuniones de planificación
        
        4. (Extra 🎁) Estima el esfuerzo de los tickets de trabajo usando la metodología (fibonacci, poker, tallas de camiseta) y unidades (horas, puntos de historia) que prefieras.
        
        En los siguientes prompts vamos a ir resolviendo cada uno de los puntos aisladamente.
        ```
        
    2. Respuesta
        
        ```markdown
        Perfecto, ahora que tengo el contexto claro, estoy listo para comenzar con la primera tarea de generar las User Stories. Avísame cuando quieras que empecemos, o si necesitas algún detalle adicional para darles forma.
        ```
        

## Solución del ejercicio

### 1. Creación de Historias de Usuario

1. Prompt
    
    ```markdown
    Vamos a comenzar a resolver el primer punto: Crea 4 historias de usuario en base al documento suministrado(la lista de principales funcionalidades y casos de uso), siguiendo la siguiente estructura:
    
    Título de la Historia de Usuario: 
    
    Como [rol del usuario],
    quiero [acción que desea realizar el usuario],
    para que [beneficio que espera obtener el usuario].
    Criterios de Aceptación:
    
    [Detalle específico de funcionalidad]
    [Detalle específico de funcionalidad]
    [Detalle específico de funcionalidad]
    Notas Adicionales:
    
    [Cualquier consideración adicional]
    Historias de Usuario Relacionadas:
    
    [Relaciones con otras historias de usuario]
    ```
    
2. Respuesta
    
    ```markdown
    Aquí tienes cuatro historias de usuario basadas en las funcionalidades clave y casos de uso del documento suministrado:
    
    Título de la Historia de Usuario: Publicación de vacantes
    
    Como reclutador,
    quiero publicar nuevas vacantes en múltiples plataformas desde una única interfaz,
    para que las ofertas de trabajo lleguen a un mayor número de candidatos calificados.
    
    Criterios de Aceptación:
    
    	•	El reclutador puede acceder a un formulario de publicación de vacantes donde ingresa título, descripción, requisitos y fecha de cierre.
    	•	El reclutador puede seleccionar las plataformas en las que desea publicar (sitio web, redes sociales, bolsas de trabajo).
    	•	El sistema valida que todos los campos obligatorios estén completos antes de publicar.
    
    Notas Adicionales:
    
    	•	Validar que la plataforma de destino esté disponible y activa antes de confirmar la publicación.
    
    Historias de Usuario Relacionadas:
    
    	•	Aplicación a vacante
    
    Título de la Historia de Usuario: Aplicación a vacante
    
    Como candidato,
    quiero postularme a vacantes publicadas en el sistema,
    para que pueda ser considerado para posiciones que se ajusten a mi perfil.
    
    Criterios de Aceptación:
    
    	•	El candidato puede buscar vacantes disponibles y ver la descripción de cada una.
    	•	El candidato puede cargar su CV y otros documentos requeridos para la aplicación.
    	•	El sistema envía una confirmación al candidato al completar la aplicación y la registra en la base de datos.
    
    Notas Adicionales:
    
    	•	Incluir validación de formato y tamaño para documentos adjuntos.
    
    Historias de Usuario Relacionadas:
    
    	•	Publicación de vacantes
    	•	Revisión y clasificación de candidatos
    
    Título de la Historia de Usuario: Revisión y clasificación de candidatos
    
    Como reclutador,
    quiero revisar y clasificar las aplicaciones de los candidatos,
    para que pueda identificar y avanzar a los perfiles más calificados en el proceso de selección.
    
    Criterios de Aceptación:
    
    	•	El reclutador puede ver una lista de candidatos postulados para cada vacante específica.
    	•	El reclutador puede aplicar filtros (experiencia, habilidades, etc.) para clasificar los perfiles.
    	•	El sistema permite actualizar el estado del candidato (preseleccionado, rechazado, en revisión) con un solo clic.
    
    Notas Adicionales:
    
    	•	Permitir comentarios internos que solo el equipo de reclutamiento puede ver en el perfil del candidato.
    
    Historias de Usuario Relacionadas:
    
    	•	Publicación de vacantes
    	•	Aplicación a vacante
    
    Título de la Historia de Usuario: Seguimiento del proceso de selección
    
    Como administrador de recursos humanos,
    quiero hacer un seguimiento en tiempo real del estado de cada candidato,
    para que pueda monitorear la eficiencia del proceso de selección y tomar decisiones informadas.
    
    Criterios de Aceptación:
    
    	•	El administrador puede ver el estado y la fase actual de cada candidato en un panel de seguimiento.
    	•	El sistema muestra métricas clave (por ejemplo, tiempo promedio para cubrir vacantes, número de candidatos en cada fase).
    	•	El administrador puede generar reportes sobre el proceso de selección con filtros personalizables.
    
    Notas Adicionales:
    
    	•	Los reportes deben poder descargarse en formato PDF y CSV.
    
    Historias de Usuario Relacionadas:
    
    	•	Revisión y clasificación de candidatos
    	•	Publicación de vacantes
    ```
    

### 2. Product Backlog - Priorización de historias de usuario

1. Prompt
    
    ```markdown
    Teniendo en cuenta las historias de usuario generadas en el prompt anterior, estima por cada item en el backlog (genera una tabla markdown):
    
    Impacto en el usuario y valor del negocio.
    Urgencia basada en tendencias del mercado y feedback de usuarios.
    Complejidad y esfuerzo estimado de implementación.
    Riesgos y dependencias entre tareas.
    ```
    
2. Respuesta
    
    ```markdown
    Aquí tienes la tabla con la estimación para cada ítem del backlog:
    
    | Historia de Usuario | Impacto en el usuario y valor del negocio | Urgencia (tendencias/feedback) | Complejidad y esfuerzo estimado | Riesgos y dependencias |
    | --- | --- | --- | --- | --- |
    | **Publicación de vacantes** | Alto: permite a los reclutadores publicar en múltiples plataformas, aumentando la visibilidad de las vacantes. | Alta: se espera que los reclutadores necesiten llegar a un mayor número de candidatos rápidamente. | Media: se requiere integración con varias plataformas. | Riesgo: cambios en API de plataformas externas. Dependencia: integración con plataformas de empleo. |
    | **Aplicación a vacante** | Alto: los candidatos pueden aplicar de manera fácil, mejorando su experiencia y aumentando el alcance de las vacantes. | Alta: se basa en el feedback de candidatos que buscan simplicidad en el proceso de aplicación. | Media: manejo de archivos adjuntos y confirmación. | Riesgo: problemas de almacenamiento y validación de archivos. Dependencia: publicación de vacantes. |
    | **Revisión y clasificación de candidatos** | Muy alto: agiliza la selección, lo que permite identificar y avanzar candidatos calificados rápidamente. | Alta: los reclutadores necesitan esta funcionalidad para optimizar el tiempo de revisión. | Alta: lógica de clasificación y filtros personalizados. | Riesgo: errores de clasificación. Dependencia: publicación y aplicación de vacantes. |
    | **Seguimiento del proceso de selección** | Muy alto: mejora el monitoreo del proceso de selección y permite tomar decisiones basadas en datos. | Media: responde a la demanda de una gestión integral del flujo de candidatos en RRHH. | Alta: generación de reportes y análisis de datos. | Riesgo: complejidad en cálculos de métricas. Dependencia: revisión y clasificación de candidatos. |
    
    Esta tabla permite tener una visión clara de los factores clave y priorizar las historias de usuario en función del valor y esfuerzo estimado.
    ```
    

### 3. Tickets de Trabajo - Selección de una user story para crear los tickets de trabajo

1. Prompt
    
    ```markdown
    Continuamos con el siguiente punto (el tercero), toma como base la primera historia de usuario priorizada en la tabla anterior(publicación de vacantes), para crear los tickets de trabajo en formato markdown, crea los tickets que consideres necesarios. Usa como referencia el siguiente ejemplo de ticket de trabajo:
    
    Título: Implementación de Autenticación de Dos Factores (2FA)
    
    Descripción: Añadir autenticación de dos factores para mejorar la seguridad del login de usuarios. Debe soportar aplicaciones de autenticación como Authenticator y mensajes SMS.
    
    Criterios de Aceptación:
    
    Los usuarios pueden seleccionar 2FA desde su perfil.
    Soporte para Google Authenticator y SMS.
    Los usuarios deben confirmar el dispositivo 2FA durante la configuración.
    Prioridad: Alta
    
    Estimación: 8 puntos de historia
    
    Asignado a: Equipo de Backend
    
    Etiquetas: Seguridad, Backend, Sprint 10
    
    Comentarios: Verificar la compatibilidad con la base de usuarios internacionales para el envío de SMS.
    
    Enlaces: Documento de Especificación de Requerimientos de Seguridad
    
    Historial de Cambios:
    
    01/10/2023: Creado por [nombre]
    05/10/2023: Prioridad actualizada a Alta por [nombre]
    ```
    
2. Respuesta
    
    ```markdown
    Aquí tienes los tickets de trabajo para la historia de usuario “Publicación de vacantes”:
    
    Título: Implementación del formulario de publicación de vacantes
    
    Descripción:
    Desarrollar un formulario de usuario en la interfaz de reclutadores para publicar nuevas vacantes. El formulario debe incluir los campos de título, descripción, requisitos y fecha de cierre, permitiendo capturar todos los detalles necesarios de la vacante.
    
    Criterios de Aceptación:
    
    	•	El formulario contiene campos para título, descripción, requisitos y fecha de cierre.
    	•	La interfaz muestra mensajes de error cuando faltan campos obligatorios.
    	•	El formulario es accesible desde el menú principal de la interfaz de reclutadores.
    
    Prioridad: Alta
    
    Estimación: 5 puntos de historia
    
    Asignado a: Equipo de Frontend
    
    Etiquetas: Frontend, UI, Publicación de Vacantes, Sprint 1
    
    Comentarios: Revisar lineamientos de diseño y accesibilidad para el formulario.
    
    Historial de Cambios:
    
    	•	04/11/2024: Creado por [nombre]
    
    Título: Implementación de validación y guardado de datos de vacante
    
    Descripción:
    Crear la lógica para validar los datos ingresados en el formulario de publicación y guardarlos en la base de datos. Asegurarse de que todos los campos requeridos estén completos y en el formato adecuado antes de enviar la vacante.
    
    Criterios de Aceptación:
    
    	•	Validación de campos obligatorios: título, descripción y fecha de cierre.
    	•	Mensajes de error específicos para cada campo incompleto o en formato incorrecto.
    	•	Al enviar el formulario, los datos se almacenan correctamente en la base de datos de vacantes.
    
    Prioridad: Alta
    
    Estimación: 6 puntos de historia
    
    Asignado a: Equipo de Backend
    
    Etiquetas: Backend, Validación de Datos, Publicación de Vacantes, Sprint 1
    
    Comentarios: Asegurarse de manejar correctamente errores de formato en el backend.
    
    Historial de Cambios:
    
    	•	04/11/2024: Creado por [nombre]
    
    Título: Integración de la publicación con plataformas externas
    
    Descripción:
    Desarrollar la funcionalidad que permita a los reclutadores distribuir sus vacantes en plataformas de empleo externas (p. ej., LinkedIn, Indeed) desde el sistema ATS.
    
    Criterios de Aceptación:
    
    	•	Los reclutadores pueden seleccionar las plataformas de publicación desde el formulario de vacantes.
    	•	Confirmación de publicación exitosa o fallida para cada plataforma seleccionada.
    	•	La interfaz de usuario muestra un resumen del estado de cada publicación externa.
    
    Prioridad: Alta
    
    Estimación: 8 puntos de historia
    
    Asignado a: Equipo de Integración
    
    Etiquetas: Integración, API, Publicación de Vacantes, Sprint 2
    
    Comentarios: Verificar las limitaciones y cuotas de API en cada plataforma externa.
    
    Historial de Cambios:
    
    	•	04/11/2024: Creado por [nombre]
    
    Título: Notificaciones de confirmación para publicaciones de vacantes
    
    Descripción:
    Implementar notificaciones para informar al reclutador sobre el estado de su vacante publicada, incluyendo confirmaciones y errores de publicación en plataformas externas.
    
    Criterios de Aceptación:
    
    	•	Notificaciones automáticas para el reclutador cuando la vacante se publique o falle.
    	•	Cada notificación incluye el estado y detalles relevantes sobre la plataforma de publicación.
    	•	Notificaciones visibles en el tablero de actividades del reclutador.
    
    Prioridad: Media
    
    Estimación: 4 puntos de historia
    
    Asignado a: Equipo de Backend
    
    Etiquetas: Notificaciones, Backend, Publicación de Vacantes, Sprint 2
    
    Comentarios: Considerar la integración con el módulo de notificaciones ya existente en la plataforma.
    
    Historial de Cambios:
    
    	•	04/11/2024: Creado por [nombre]
    
    Estos tickets cubren las tareas clave para implementar la funcionalidad de publicación de vacantes de manera efectiva.
    ```
    

### 4. Estimación de esfuerzo de tickets de trabajo

1. Prompt
    
    ```markdown
    Dime que estrategia usaste para estimar el esfuerzo en puntos de historia, de los tickets de trabajo que acabaste de generar
    ```
    
2. Respuesta
    
    ```markdown
    Para estimar el esfuerzo en puntos de historia, utilicé la metodología de Fibonacci, que se basa en una secuencia de números donde cada número es la suma de los dos anteriores (1, 2, 3, 5, 8, etc.). Este enfoque es útil para reflejar la incertidumbre creciente en tareas más complejas.
    
    La estrategia específica que apliqué fue:
    
    	1.	Analizar la complejidad técnica: Evalué cada ticket en función de la cantidad de trabajo técnico necesario, como integración con APIs externas o validación de datos, lo cual aumenta el esfuerzo debido a la complejidad o posibles dependencias.
    	2.	Considerar los criterios de aceptación y dependencias: Tareas con múltiples criterios de aceptación o que involucran otras funcionalidades (como notificaciones dependientes de la publicación) se puntuaron con valores más altos, ya que requerirían un esfuerzo coordinado entre equipos.
    	3.	Asignación de puntos con Fibonacci:
    	•	Tareas simples o directas (p. ej., crear formularios con validación básica) recibieron estimaciones más bajas, como 4 o 5 puntos.
    	•	Tareas de complejidad moderada (como la integración con plataformas externas) fueron estimadas en 8 puntos, reflejando los desafíos de integrar y manejar la variabilidad en las APIs externas.
    	•	La prioridad no afectó directamente los puntos de historia, pero tareas prioritarias se asignaron a los primeros sprints para asegurar la entrega temprana de valor.
    
    Este enfoque en la secuencia de Fibonacci ayudó a capturar tanto el esfuerzo técnico como las incertidumbres, distribuyendo la carga de trabajo de manera proporcional al esfuerzo estimado para cada ticket.
    ```