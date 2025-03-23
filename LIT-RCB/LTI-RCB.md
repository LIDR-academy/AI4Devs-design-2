# Documentación Proyecto LTI

## Descripción del Software

El software LTI es un sistema avanzado de seguimiento de candidatos (ATS - Applicant Tracking System) diseñado para revolucionar el proceso de reclutamiento. Maximiza eficiencia, fomenta la colaboración en tiempo real, automatiza tareas repetitivas y brinda asistencia inteligente con IA.

### Valor añadido y ventajas competitivas
- **Automatización inteligente:** Reducción de tareas manuales.
- **Colaboración en tiempo real:** Comunicación fluida entre equipos.
- **Asistencia IA:** Análisis predictivos y recomendaciones para selección.
- **Interfaz intuitiva:** Experiencia de usuario mejorada.

## Funciones Principales

- Gestión integral de candidatos
- Automatización de reclutamiento
- Colaboración en tiempo real
- Reportes avanzados
- Integraciones externas (LinkedIn, Indeed, Slack)

## Lean Canvas

| Problema | Clientes | Propuesta de valor |
|----------|----------|---------------------|
| Procesos lentos y decisiones poco optimizadas | HR, Reclutadores, Managers | Automatización IA y colaboración en tiempo real |

| Solución | Canales | Ingresos |
|----------|---------|----------|
| Automatización, IA, Dashboard | Web, API | Suscripción mensual, planes empresariales |

| Costes | Métricas | Ventajas injustas |
|--------|----------|-------------------|
| IA, servidores, marketing | Adopción, satisfacción usuario | IA avanzada y colaboración superior |

```mermaid
graph TD
Problema[Procesos lentos y decisiones poco optimizadas] --> Clientes[HR, Reclutadores, Managers]
Clientes --> Propuesta[Automatización IA, colaboración en tiempo real]
Propuesta --> Solucion[Automatización, IA, Dashboard colaborativo]
Solución --> Canales[Web, API]
Canales --> Ingresos[Suscripción mensual, Planes empresariales]
Ingresos --> Costes[IA, servidores, marketing]
Costes --> Metricas[Adopción, satisfacción usuario]
Metricas --> Ventajas[IA avanzada, colaboración superior]
```
## Casos de Uso Principales

### Caso de Uso 1: Gestión de candidatos
- Actor: Reclutador
- Descripción: Maneja candidatos desde recepción de CV hasta contratación.
```mermaid
graph TD
Reclutador --> Recepción_CV --> Revisión_CV --> Entrevistas --> Contratación
```

### Caso de uso 2: Colaboración en tiempo real
- Actor: Gerente, Reclutador
- Descripción: Evaluación conjunta de candidatos mediante comentarios en tiempo real.
```mermaid
graph TD
Gerente --> Colaboracion[Evaluación conjunta]
Reclutador --> Colaboración
Colaboracion --> ComentariosTiempoReal
ComentariosTiempoReal --> Notificaciones
```

### Caso de uso 3: Reportes Inteligentes
- Actor: Gerente HR
- Descripción: Generación automática de informes predictivos usando IA.

```mermaid
graph TD
GerenteHR --> SolicitudReporte
SolicitudReporte --> GeneracionReporteIA
GeneracionReporteIA --> InformePredictivo
```

## Modelo de datos

- **Candidato:**
  - ID (UUID)
  - Nombre (String)
  - Email (String)
  - Teléfono (String)
  - Estado (Enum)
  - Fecha de aplicación (Date)
  - CV (File)

- **Vacante:**
  - ID (UUID)
  - Título (String)
  - Descripción (Text)
  - Estado (Enum)

- **Reclutador:**
  - ID (UUID)
  - Nombre (String)
  - Email (String)

- **Comentario:**
  - ID (UUID)
  - Contenido (Text)
  - Fecha (Timestamp)
  - Autor (UUID)

### Relaciones:
- Vacante → Reclutador (1 a muchos)
- Vacante ↔ Candidato (muchos a muchos)
- Candidato → Comentario (1 a muchos)
- Reclutador → Comentario (1 a muchos)

```mermaid
erDiagram
Candidato ||--o{ Comentario : "tiene comentarios"
Vacante ||--o{ Reclutador : gestionado_por
Vacante }|..|{ Candidato : postulan
Reclutador ||--o{ Comentario : genera

Candidato {
UUID id
String nombre
String email
String telefono
Enum estado
Date fecha_aplicacion
File CV
}

Vacante {
UUID id
String titulo
String descripcion
Enum estado
}

Reclutador {
UUID id
String nombre
String email
}

Comentario {
UUID id
Text contenido
Timestamp fecha
UUID autor
}
```

## Diseño del Sistema Alto Nivel

Arquitectura basada en microservicios:

- **Front-end:** Angular
- **Back-end:** Microservicios REST con Java Spring Boot
- **Base de datos:** PostgreSQL
- **Seguridad:** JWT, OAuth2
- **Integraciones:** APIs externas



### Diagrama Alto Nivel

```mermaid
graph TD
Usuario --> Frontend[Angular]
Frontend --> GatewayAPI
Gateway_API --> MicroservicioCandidatos
Gateway_API --> MicroservicioIA
Microservicio_Candidatos --> BaseDatos[(PostgreSQL)]
Microservicio_IA --> BaseDatos
Gateway_API --> IntegracionesExternas
```

## Diagrama C4

### Nivel 1: Sistema (Contexto)

- **LTI ATS:** Aplicación web para reclutamiento
  - **Usuarios:** Reclutadores, Gerentes
  - **Sistemas externos:** LinkedIn, Slack, Indeed

### Nivel 2: Contenedores

- **Web App (Angular)**
- **Microservicio Gestión de Candidatos (Spring Boot)**
- **Microservicio IA (Spring Boot)**
- **Base de datos (PostgreSQL)**

```mermaid
graph TD
Usuario --> WebApp[Aplicación Web Angular]
WebApp --> GatewayAPI
GatewayAPI --> MicroservicioCandidatos[Microservicio Gestión de Candidatos]
GatewayAPI --> MicroservicioIA[Microservicio IA]
Microservicio_Candidatos --> PostgreSQL[(Base de Datos)]
Microservicio_IA --> PostgreSQL
GatewayAPI --> APIsExternas[LinkedIn, Slack, Indeed]
```

### Nivel 2: Componentes

- **Controlador REST:** Peticiones HTTP.
- **Servicio de Negocio:** Gestión lógica.
- **Repositorio Datos:** Acceso PostgreSQL.
- **Cliente API:** Integración con externos.

### Nivel 3: Componentes específicos

- **CandidatoService:** Gestión lógica candidatos.
- **ComentarioService:** Gestión comentarios.
- **EmailNotificationService:** Emails automáticos.


```mermaid
graph TD
ControladorREST --> ServicioNegocio
ServicioNegocio --> RepositorioDatos[Repositorio PostgreSQL]
ServicioNegocio --> ClienteAPI
ClienteAPI --> LinkedIn
ClienteAPI --> Indeed
```
