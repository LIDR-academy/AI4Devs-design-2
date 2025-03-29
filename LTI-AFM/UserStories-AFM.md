
# 📘 LTI – Documentación Técnica: Aplicación de Candidatos y Prueba Gamificada


## 📚 Historias de Usuario (Resumen)

---

### 🧑‍💼 Historia de Usuario 1: Publicación de vacante

**Como** reclutador,  
**quiero** crear y publicar una oferta laboral desde el panel de administración,  
**para que** pueda comenzar a recibir postulaciones de candidatos calificados.

**Criterios de aceptación**:
- El formulario debe incluir título, descripción, tipo de contrato, ubicación (si aplica) y competencias clave.
- Puede habilitarse la evaluación automática con gamificación.
- Debe poder asociarse a una campaña o fase del proceso de selección.

---

### 👩‍💻 Historia de Usuario 2: Aplicación del candidato y prueba gamificada

**Como** candidato,  
**quiero** aplicar fácilmente a una vacante y completar una prueba gamificada,  
**para que** pueda demostrar mis habilidades de forma interactiva y obtener mayor visibilidad.

---

### 🧑‍💼 Historia de Usuario 3: Visualización de pipeline de selección

**Como** reclutador,  
**quiero** visualizar todos los candidatos en un pipeline por etapas (kanban),  
**para que** pueda gestionar fácilmente en qué punto se encuentra cada postulación.

**Criterios de aceptación**:
- Las etapas incluyen: Postulado, Evaluación, Entrevista, Oferta, Contratado/Descartado.
- Se puede arrastrar un candidato entre etapas.
- Cada ficha muestra el nombre, puntaje, estatus y notas internas.

---

### 🧾 Historia de Usuario 4: Validación de credenciales con blockchain

**Como** administrador de selección,  
**quiero** verificar automáticamente las credenciales educativas y laborales por blockchain,  
**para que** pueda asegurarme de que la información de los candidatos es real.

**Criterios de aceptación**:
- El sistema valida documentos académicos y laborales usando un tercero (blockchain).
- Muestra resultado de validación en el perfil del candidato: Verificado / No verificado.
- Debe permitir al candidato subir un nuevo documento si se requiere.

---

### 🌐 Historia de Usuario 5: Métricas de diversidad e inclusión

**Como** analista de diversidad e inclusión,  
**quiero** visualizar estadísticas anónimas sobre la diversidad en los procesos de selección,  
**para que** pueda detectar sesgos y mejorar nuestras políticas de contratación.

**Criterios de aceptación**:
- Se muestran métricas agregadas (género, edad, localización, nivel educativo, etc.).
- Los datos deben estar anonimizados y cumplir normativas de protección de datos.
- Se pueden comparar entre campañas, periodos o equipos de reclutamiento.

---

## 🗂️ Backlog Técnico Priorizado – Método RICE

| Tarea Técnica           | Reach | Impact | Conf. | Effort | RICE Score | Comentario |
|-------------------------|--------|--------|--------|--------|-------------|------------|
| `auth-usuarios`         | 1000   | 2.0    | 90%    | 5      | **360**     | Fundamental para todo |
| `vacante-model`         | 1000   | 1.5    | 95%    | 3      | **475**     | Base del sistema |
| `vacante-api`           | 1000   | 1.5    | 90%    | 4      | **337.5**   | Bloque para UI y postulaciones |
| `vacante-ui`            | 1000   | 1.2    | 85%    | 4      | **255**     | Visible en demo inicial |
| `registro-candidato`    | 1000   | 1.5    | 90%    | 3      | **450**     | Punto de entrada del usuario |
| `kanban-ui`             | 300    | 2.0    | 80%    | 4      | **120**     | Aporta claridad a recruiters |
| `pipeline-api`          | 300    | 1.5    | 85%    | 3      | **127.5**   | Back del tablero de flujo |
| `prueba-gamificada-ui`  | 500    | 2.0    | 70%    | 6      | **116.7**   | Diferenciador del producto |
| `evaluador-backend`     | 500    | 1.5    | 70%    | 6      | **87.5**    | Necesario para pruebas automáticas |
| `registro-respuestas`   | 500    | 1.0    | 85%    | 3      | **141.6**   | Almacén de datos clave |
| `control-acceso-api`    | 1000   | 1.2    | 90%    | 2      | **540**     | Seguridad rápida de implementar |
| `proteccion-datos`      | 1000   | 2.0    | 80%    | 6      | **266.7**   | Crítico para confianza y escalado |
| `resultados-dashboard`  | 200    | 1.2    | 80%    | 3      | **64**      | Se puede diferir |
| `verificador-blockchain`| 100    | 2.0    | 60%    | 7      | **17.1**    | Se puede implementar post-MVP |

---

## 🎯 Historia de Usuario 2

**Como** candidato,  
**quiero** aplicar fácilmente a una vacante y completar una prueba gamificada,  
**para que** pueda demostrar mis habilidades de forma interactiva y obtener mayor visibilidad.

---

## 🧩 Épica: Postulación de Candidato + Prueba Gamificada

### 🔹 Ticket 1: `POST /api/apply-to-job`
**Nombre**: Crear endpoint de aplicación a vacante  
**Descripción**: Permitir que un candidato (con o sin login) se postule a una vacante, almacenando la información mínima y generando un identificador de sesión de evaluación.  
**Criterios técnicos**:
- Recibe `job_id`, `nombre`, `email`, `cv_url`, `linkedin_url` (opcional).
- Crea entrada en tabla `applications`.
- Devuelve `application_id` y si la vacante tiene prueba activa.
- Debe validar duplicados por email + job_id.

**Dependencias**: `vacante-model`, `auth opcional`  
**Esfuerzo estimado**: 3 puntos  
**Validación QA**:  
- Se puede aplicar sin cuenta  
- La aplicación se registra y es visible para el reclutador  
- No se permite duplicado

---

### 🔹 Ticket 2: `GET /api/jobs/:id/check-gamification`
**Nombre**: Determinar si la vacante tiene prueba gamificada  
**Descripción**: Devuelve si la vacante asociada tiene configurada una prueba, el tipo de prueba y su duración.  
**Criterios técnicos**:
- Devuelve `{ hasGame: true, gameType: "quiz", duration: 300 }`
- Valida que el juego esté activo en el backend

**Dependencias**: `vacante-model` + configuración gamificada  
**Esfuerzo estimado**: 1 punto  
**Validación QA**:  
- Vacantes sin prueba devuelven `hasGame: false`

---

### 🔹 Ticket 3: `Pantalla: Aplicación + Inicio de prueba`
**Nombre**: Formulario de aplicación y redirección a prueba gamificada  
**Descripción**: Crear UI para aplicación del candidato y, si hay prueba, mostrar botón “Iniciar prueba”.  
**Criterios técnicos**:
- Recolecta los datos básicos (nombre, correo, CV)  
- Valida campos antes de enviar  
- Redirige automáticamente a la pantalla de la prueba si está activa  

**Tecnologías**: React + Tailwind (o stack actual)  
**Esfuerzo estimado**: 3 puntos  
**Dependencias**: Ticket 1 + Ticket 2  
**Validación QA**:
- El formulario no se puede enviar vacío  
- Aparece el botón de “Iniciar prueba” si aplica

---

### 🔹 Ticket 4: `Pantalla: Prueba gamificada (UI)`
**Nombre**: Renderizado de prueba gamificada tipo quiz  
**Descripción**: Crear componente para mostrar preguntas tipo test una a una, con cronómetro y control de navegación.  
**Criterios técnicos**:
- Lee las preguntas desde el backend
- Timer cuenta regresiva visible
- Una sola respuesta por pregunta
- Al finalizar, autoenvía las respuestas

**Notas para dev**:
- Usar `useEffect` para temporizador
- Cada pregunta puede tener 3–5 opciones

**Dependencias**: Backend ya tenga mock de preguntas  
**Esfuerzo estimado**: 5 puntos  
**Validación QA**:
- No se puede pasar sin responder  
- El tiempo se respeta  
- Al final muestra mensaje de “¡Gracias!”

---

### 🔹 Ticket 5: `POST /api/gamification/submit`
**Nombre**: Guardar respuestas y calcular resultado  
**Descripción**: Backend recibe respuestas, calcula el puntaje y marca la aplicación como completada.  
**Criterios técnicos**:
- Validar respuestas contra clave correcta
- Calcular puntaje (ej: 1 por correcta)
- Guardar en `application_results` o similar
- Emitir evento `evaluation.completed`

**Esfuerzo estimado**: 3 puntos  
**Dependencias**: Ticket 1 + respuestas de prueba  
**Validación QA**:
- Se guarda el puntaje correctamente  
- Aparece en el dashboard del reclutador

---

### 🔹 Ticket 6: `GET /api/recruiter/dashboard/applications`
**Nombre**: Ver resultados de candidatos en dashboard  
**Descripción**: Incluir puntaje de prueba en la vista de aplicaciones del reclutador.  
**Criterios técnicos**:
- Agregar campo `score` o `gamificationStatus`
- Permitir orden por mayor puntaje  

**Esfuerzo estimado**: 2 puntos  
**Dependencias**: Ticket 5  
**Validación QA**:
- El puntaje aparece correctamente al aplicar filtros

---

## 🧠 Metodología de Estimación de Esfuerzo

Se utilizó la técnica de **Story Points** (escala Fibonacci: 1, 2, 3, 5, 8) para estimar esfuerzo relativo.  
Cada ticket fue evaluado por:
- Reutilización
- Complejidad lógica y visual
- Dependencias técnicas
- Incertidumbre
- Riesgo de integración

---

## ✅ Siguiente paso sugerido

Este archivo puede usarse como:
- Documento base para planificación de sprints
- Fuente para importar tickets en Jira, Linear, Trello, Notion, etc.
- Material de onboarding técnico para nuevos miembros del equipo

---

**Autor**: Felipe (con apoyo de ChatGPT como Product Manager y Business Analyst)  
**Fecha**: Marzo 2025
