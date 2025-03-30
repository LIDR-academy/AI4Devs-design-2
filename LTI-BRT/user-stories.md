
```markdown
# Historia de usuario
Como reclutador quiero poder crear y publicar ofertas de empleo en múltiples plataformas con un solo clic para aumentar la visibilidad de las vacantes y atraer más candidatos cualificados.

# Criterios de aceptación
1. El sistema debe permitir al reclutador ingresar título, descripción, requisitos, ubicación y tipo de contrato.
2. La IA debe sugerir mejoras en el contenido de la oferta antes de publicarla.
3. El reclutador puede seleccionar múltiples plataformas (LinkedIn, Indeed, Glassdoor) para su publicación.
4. El ATS debe mostrar una vista previa antes de confirmar la publicación.
5. Se deben mostrar métricas de rendimiento como número de vistas y postulaciones en tiempo real.

## Notas adicionales 
Las recomendaciones de la IA deben basarse en patrones históricos de éxito y keywords relevantes al sector.

## Historias de usuario relacionadas
- Evaluación automática de candidatos con IA.
- Seguimiento de métricas de publicaciones.
```

---

```markdown
# Historia de usuario
Como reclutador quiero recibir automáticamente un ranking de candidatos basado en su compatibilidad con la oferta para reducir el tiempo invertido en revisar currículums manualmente.

# Criterios de aceptación
1. El sistema debe analizar la información de los candidatos recibida desde plataformas externas o subida directamente.
2. El motor de IA debe generar una puntuación de compatibilidad basada en experiencia, habilidades y formación.
3. Debe presentarse un ranking ordenado con filtros por puntuación, experiencia y habilidades.
4. El reclutador debe poder revisar el perfil estructurado del candidato desde el sistema.
5. El sistema debe permitir al reclutador iniciar el proceso de entrevista o prueba técnica desde el mismo flujo.

## Notas adicionales 
El análisis semántico debe ser capaz de detectar sinónimos y contexto de las habilidades, no solo coincidencias literales.

## Historias de usuario relacionadas
- Coordinación de entrevistas y evaluación colaborativa.
```

---

```markdown
# Historia de usuario
Como reclutador quiero poder agendar entrevistas automáticamente con base en la disponibilidad del equipo y del candidato para agilizar la coordinación del proceso.

# Criterios de aceptación
1. El sistema debe consultar las agendas de los entrevistadores desde Google Calendar, Outlook u otro calendario vinculado.
2. El candidato debe recibir una notificación automática con detalles y confirmación de la entrevista.
3. El reclutador debe poder incluir un formulario de evaluación para la entrevista.
4. Los entrevistadores deben poder tomar notas y calificar al candidato desde el sistema durante la entrevista.
5. Debe consolidarse un reporte de feedback con las evaluaciones del equipo.

## Notas adicionales 
Las entrevistas pueden ser presenciales o virtuales; en caso de ser virtuales, debe incluirse un enlace a Zoom, Teams o similar.

## Historias de usuario relacionadas
- Evaluación estructurada de candidatos.
- Feedback colaborativo posterior a entrevistas.
```

---

```markdown
# Historia de usuario
Como candidato quiero tener acceso a un portal donde pueda ver el estado de mis postulaciones en tiempo real para tener claridad sobre mi proceso de selección.

# Criterios de aceptación
1. El portal debe mostrar una lista de todas las postulaciones realizadas por el candidato.
2. Cada postulación debe tener un estado visible (en revisión, entrevista agendada, descartado, etc.).
3. Debe haber un historial de comunicaciones automatizadas (emails enviados por el sistema).
4. El sistema debe permitir enviar notificaciones personalizadas por cada cambio de estado.
5. El candidato debe poder confirmar o rechazar entrevistas directamente desde el portal.

## Notas adicionales 
Un chatbot puede ser utilizado para resolver dudas frecuentes del candidato y mejorar la experiencia.

## Historias de usuario relacionadas
- Coordinación de entrevistas.
- Automatización de comunicaciones con candidatos.
```

---

```markdown
# Historia de usuario
Como gerente de recursos humanos quiero visualizar dashboards con KPIs clave del proceso de selección para tomar decisiones basadas en datos y optimizar nuestras estrategias de reclutamiento.

# Criterios de aceptación
1. El sistema debe ofrecer visualización de indicadores como tiempo promedio de contratación, tasa de conversión por fuente y número de postulantes.
2. Los datos deben poder filtrarse por puesto, departamento, fecha y reclutador.
3. El sistema debe predecir la tasa de éxito de un candidato con base en datos históricos.
4. Debe incluirse un módulo de análisis de diversidad e inclusión.
5. Los reportes deben ser exportables (PDF, Excel) y compartirlos con otros stakeholders.

## Notas adicionales 
La capacidad de personalizar los dashboards es clave para adaptarse a las necesidades específicas del negocio.

## Historias de usuario relacionadas
- Evaluación con IA de candidatos.
- Publicación de ofertas y análisis de rendimiento.
```

---

# 🥇 Prioridad 1 - Ranking automático de candidatos con IA

**Motivo de Prioridad:**
Esta funcionalidad representa el mayor diferencial del sistema LTI ATS frente a otros ATS tradicionales. La automatización del análisis y ranking de candidatos tiene un **alto impacto en la eficiencia** del proceso de selección. A pesar de que tiene un esfuerzo medio-alto, es clave para la propuesta de valor y debe abordarse pronto.

**Esfuerzo estimado:** 8 Story Points  
**Stack sugerido:**  
- Backend: Node.js + PostgreSQL (motor de IA y reglas de negocio)  
- Procesamiento asíncrono: RabbitMQ (evaluación en segundo plano)  
- Frontend: React + Typescript (visualización del ranking y filtros)

---

# 🥈 Prioridad 2 - Creación y publicación automática de ofertas

**Motivo de Prioridad:**
Es la funcionalidad de entrada para cualquier flujo de reclutamiento. Tiene un impacto muy alto porque **activa el sistema** y permite generar tráfico de candidatos. Además, puede ser desarrollada rápidamente con el stack actual.

**Esfuerzo estimado:** 5 Story Points  
**Stack sugerido:**  
- Backend: PHP (Symfony) para formularios y lógica de publicación  
- Integraciones: Node.js para publicar en APIs de terceros (LinkedIn, Indeed)  
- Frontend: React + Typescript para formularios y previsualización

---

# 🥉 Prioridad 3 - Coordinación de entrevistas con integración de calendarios

**Motivo de Prioridad:**
Tiene un impacto medio-alto al reducir fricciones internas en la organización y mejorar la experiencia del candidato. Su implementación depende de integraciones externas, pero se puede comenzar con herramientas como Google Calendar.

**Esfuerzo estimado:** 8 Story Points  
**Stack sugerido:**  
- Backend: Node.js para manejar disponibilidad y enlaces de videollamada  
- Integración con APIs externas: Google Calendar, Microsoft Graph  
- Frontend: React (para agendamiento y confirmación)

---

# 🏅 Prioridad 4 - Visualización de KPIs y dashboards de analítica

**Motivo de Prioridad:**
Esta funcionalidad es clave para usuarios avanzados (gerentes), pero no crítica para las primeras etapas del producto. Su impacto es **estratégico**, pero puede desarrollarse una vez que los flujos principales estén en funcionamiento.

**Esfuerzo estimado:** 5 Story Points  
**Stack sugerido:**  
- Backend: PostgreSQL (consultas agregadas)  
- Frontend: React + librerías de visualización (ej. Chart.js o Recharts)  
- Backend opcional: Node.js para analítica avanzada y predicción

---

# 🎖️ Prioridad 5 - Portal del candidato con estado de postulaciones

**Motivo de Prioridad:**
Aunque mejora mucho la experiencia del candidato, tiene un **impacto más bajo en el negocio** en etapas iniciales. Su desarrollo requiere una interfaz diferenciada y control de roles, lo cual implica mayor esfuerzo inicial.

**Esfuerzo estimado:** 8 Story Points  
**Stack sugerido:**  
- Frontend: Next.js (para SSR del portal público)  
- Backend: Symfony + PostgreSQL (consulta de estados, autenticación del candidato)  
- RabbitMQ para notificaciones por cambio de estado


---  



# Planificación de tareas UserStory con prioridad 1

```markdown
# Ticket #1: Diseño del modelo de datos para compatibilidad candidato-oferta

## Descripción
Definir y modelar la estructura de datos necesaria para almacenar la información de candidatos, ofertas y sus relaciones para ser utilizada por el motor de IA en la evaluación de compatibilidad.

## Criterios de aceptación
- El modelo debe incluir campos como experiencia, educación, habilidades y puntuación IA.
- Debe existir una tabla intermedia para la relación oferta-candidato con campos de evaluación.
- El diseño debe ser revisado y validado por el Tech Lead.

## Prioridad
Crítico

## Estimación de esfuerzo
3 Story Points

## Asignado
Senior

## Categoría
Tarea Técnica

## Comentarios
Este modelo será la base para que el motor de IA funcione correctamente. Debe alinearse con el modelo de datos global del sistema.

```

---
```markdown
# Ticket #2: Parsing automático de CVs y estructuración del perfil del candidato

## Descripción
Implementar la funcionalidad para extraer información clave del CV (PDF, DOCX, etc.) y almacenarla en formato estructurado en la base de datos del sistema.

## Criterios de aceptación
- El sistema debe extraer nombre, experiencia, habilidades y formación.
- El resultado del parsing debe almacenarse en el modelo del candidato.
- Se deben registrar errores si el CV no puede ser leído correctamente.

## Prioridad
Crítico

## Estimación de esfuerzo
5 Story Points

## Asignado
Junior 1

## Categoría
Feature

## Comentarios
Se puede utilizar una librería de parsing como `pdf-parse` o `docx-parser` desde Node.js. La calidad del parsing impacta directamente en el ranking.

```

---
```markdown
# Ticket #3: Implementación del motor de puntuación de compatibilidad (IA básica)

## Descripción
Desarrollar el motor inicial que calcula una puntuación de compatibilidad entre el perfil del candidato y los requisitos de una oferta utilizando reglas definidas y similitud semántica básica.

## Criterios de aceptación
- El motor debe considerar experiencia, habilidades y educación para calcular la puntuación.
- La puntuación debe almacenarse en la tabla de relación oferta-candidato.
- Debe ser ejecutado de forma asíncrona (RabbitMQ) cuando se recibe una nueva aplicación.

## Prioridad
Crítico

## Estimación de esfuerzo
8 Story Points

## Asignado
Senior

## Categoría
Feature

## Comentarios
Este motor puede utilizar técnicas simples de NLP como comparación de keywords o TF-IDF en una primera fase. Posteriormente puede evolucionar a un modelo de ML más avanzado.

```

---
```markdown
# Ticket #4: Configuración de proceso asíncrono con RabbitMQ para análisis de compatibilidad

## Descripción
Configurar RabbitMQ y desarrollar workers que se encarguen del procesamiento de compatibilidad entre candidatos y ofertas en segundo plano.

## Criterios de aceptación
- RabbitMQ debe estar configurado y funcional en el entorno de desarrollo.
- Se debe crear una cola específica para análisis de compatibilidad.
- Los workers deben leer eventos de nuevas postulaciones y ejecutar el motor de IA.

## Prioridad
Alto

## Estimación de esfuerzo
5 Story Points

## Asignado
Tech Lead

## Categoría
Tarea Técnica

## Comentarios
El uso de colas es fundamental para evitar sobrecarga en el sistema cuando hay múltiples postulaciones en paralelo.

```

---
```markdown
# Ticket #5: Interfaz de visualización del ranking de candidatos

## Descripción
Desarrollar una interfaz que permita a los reclutadores visualizar la lista de candidatos ordenados por su puntuación de compatibilidad con una oferta específica.

## Criterios de aceptación
- La lista debe mostrar nombre, puntuación, experiencia, y botones de acción (ver perfil, invitar a entrevista).
- El orden debe estar determinado por la puntuación del motor de IA.
- Debe incluir filtros por experiencia y habilidades.

## Prioridad
Alto

## Estimación de esfuerzo
5 Story Points

## Asignado
Junior 2

## Categoría
Feature

## Comentarios
Se recomienda usar React con Typescript y estados locales para manejar filtros y ordenamientos. Este módulo debe estar accesible desde el flujo de gestión de postulaciones.

```

---
```markdown
# Ticket #6: Investigación sobre técnicas de matching semántico para perfiles laborales

## Descripción
Investigar métodos y librerías para mejorar el análisis semántico entre perfiles de candidatos y descripciones de ofertas, con foco en procesamiento de lenguaje natural (NLP).

## Criterios de aceptación
- Identificar al menos 2 técnicas viables aplicables al proyecto (ej: Word2Vec, BERT embeddings).
- Documentar ventajas y limitaciones de cada técnica.
- Proponer plan de implementación futura (MVP vs. largo plazo).

## Prioridad
Medio

## Estimación de esfuerzo
3 Story Points

## Asignado
Senior

## Categoría
Investigación

## Comentarios
Esta tarea ayudará a guiar el roadmap técnico del motor de IA a mediano/largo plazo.

```
