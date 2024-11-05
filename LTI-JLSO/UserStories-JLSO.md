# ✍️ Creación del Backlog de Producto LTI 🔴

## 1. User Stories

### 1. Publicación de vacantes

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

### 2. Aplicación a vacante

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

### 3. Revisión y clasificación de candidatos

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

### 4. Seguimiento del proceso de selección

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

## 2. Product Backlog

| Historia de Usuario | Impacto en el usuario y valor del negocio | Urgencia (tendencias/feedback) | Complejidad y esfuerzo estimado | Riesgos y dependencias |
| --- | --- | --- | --- | --- |
| **Publicación de vacantes** | Alto: permite a los reclutadores publicar en múltiples plataformas, aumentando la visibilidad de las vacantes. | Alta: se espera que los reclutadores necesiten llegar a un mayor número de candidatos rápidamente. | Media: se requiere integración con varias plataformas. | Riesgo: cambios en API de plataformas externas. Dependencia: integración con plataformas de empleo. |
| **Aplicación a vacante** | Alto: los candidatos pueden aplicar de manera fácil, mejorando su experiencia y aumentando el alcance de las vacantes. | Alta: se basa en el feedback de candidatos que buscan simplicidad en el proceso de aplicación. | Media: manejo de archivos adjuntos y confirmación. | Riesgo: problemas de almacenamiento y validación de archivos. Dependencia: publicación de vacantes. |
| **Revisión y clasificación de candidatos** | Muy alto: agiliza la selección, lo que permite identificar y avanzar candidatos calificados rápidamente. | Alta: los reclutadores necesitan esta funcionalidad para optimizar el tiempo de revisión. | Alta: lógica de clasificación y filtros personalizados. | Riesgo: errores de clasificación. Dependencia: publicación y aplicación de vacantes. |
| **Seguimiento del proceso de selección** | Muy alto: mejora el monitoreo del proceso de selección y permite tomar decisiones basadas en datos. | Media: responde a la demanda de una gestión integral del flujo de candidatos en RRHH. | Alta: generación de reportes y análisis de datos. | Riesgo: complejidad en cálculos de métricas. Dependencia: revisión y clasificación de candidatos. |

## 3. Tickets de trabajo

1. Título: Implementación de Autenticación de Dos Factores (2FA)
    
    Descripción: Añadir autenticación de dos factores para mejorar la seguridad del login de usuarios. Debe soportar aplicaciones de autenticación como Authenticator y mensajes SMS.
    
    Criterios de Aceptación:
    

        •	Los usuarios pueden seleccionar 2FA desde su perfil.
        •	Soporte para Google Authenticator y SMS.
        •	Los usuarios deben confirmar el dispositivo 2FA durante la configuración.

    Prioridad: Alta
    
    Estimación: 8 puntos de historia
    
    Asignado a: Equipo de Backend
    
    Etiquetas: Seguridad, Backend, Sprint 10
    
    Comentarios: Verificar la compatibilidad con la base de usuarios internacionales para el envío de SMS.
    
    Enlaces: Documento de Especificación de Requerimientos de Seguridad
    
    Historial de Cambios:
    
    ```
    •	01/10/2023: Creado por [nombre]
    •	05/10/2023: Prioridad actualizada a Alta por [nombre]
2. Título: Implementación del formulario de publicación de vacantes
    
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
3. Título: Implementación de validación y guardado de datos de vacante
    
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
4. Título: Integración de la publicación con plataformas externas
    
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

## 4. Estimación de esfuerzo de los tickets

En el punto anterior cada ticket quedó con su estimación asociada, utilizando la metodología de Fibonacci, que se basa en una secuencia de números donde cada número es la suma de los dos anteriores (1, 2, 3, 5, 8, etc.)