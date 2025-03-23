# UserStories

## 🧩 Tipos de Usuarios

1. Reclutador
2. Manager de contratación
3. Candidato
4. Administrador de empresa
5. Sistema (automatizaciones/IA)

⸻

## 📋 Historias de Usuario por Tipo

### 🎯 Reclutador

US01 - Crear y publicar una vacante

Como reclutador, quiero crear una nueva vacante y publicarla en múltiples portales, para recibir candidatos lo antes posible.

US02 - Ver y filtrar candidatos por vacante

Como reclutador, quiero ver la lista de candidatos aplicados a una vacante, y filtrarlos por experiencia, palabras clave o skills, para enfocarme en los más adecuados.

US03 - Programar entrevistas automáticamente

Como reclutador, quiero que el sistema proponga horarios de entrevista automáticamente según la disponibilidad, para ahorrar tiempo y evitar conflictos.

US04 - Dejar comentarios sobre un candidato

Como reclutador, quiero anotar observaciones internas sobre un candidato, para compartirlas con el equipo y tomar decisiones en conjunto.

⸻

### 🧑‍💼 Manager de contratación

US05 - Revisar candidatos y dejar feedback

Como manager, quiero ver los perfiles de candidatos seleccionados y añadir feedback colaborativo, para facilitar la elección del mejor perfil.

US06 - Ver el estado del proceso de selección

Como manager, quiero tener una vista clara del estado de cada vacante, para entender en qué etapa está cada candidato.

⸻

### 🙋 Candidato

US07 - Aplicar a una vacante

Como candidato, quiero aplicar fácilmente a una vacante con mi CV y LinkedIn, para postularme sin fricciones.

US08 - Ver el estado de mi candidatura

Como candidato, quiero ver el estado actual de mi postulación, para saber si sigo en el proceso o fui descartado.

US09 - Confirmar entrevista sugerida

Como candidato, quiero recibir una notificación con la propuesta de horario de entrevista y poder confirmarla o sugerir cambios, para coordinar de manera cómoda.

⸻

### 🛠️ Administrador de empresa

US10 - Invitar nuevos usuarios

Como administrador de empresa, quiero invitar nuevos miembros al sistema, asignándoles roles, para gestionar mi equipo de reclutamiento.

US11 - Configurar canales de publicación

Como administrador, quiero configurar qué portales de empleo se conectan con LTI, para publicar vacantes desde una única plataforma.

US12 - Acceder a reportes y estadísticas

Como administrador, quiero ver métricas como tiempo promedio de contratación o número de entrevistas, para analizar el rendimiento del equipo de RRHH.

⸻

### 🤖 Sistema / Automatización / IA

US13 - Filtrar candidatos automáticamente

Como sistema, necesito analizar los CVs recibidos y filtrarlos por relevancia, para presentar primero los candidatos con mejor match.

US14 - Proponer horario óptimo de entrevista

Como sistema, necesito calcular un horario óptimo de entrevista según disponibilidad de partes involucradas, para evitar solapamientos y optimizar el tiempo.

⸻

## 🧭 Prioridad de Historias de Usuario – MoSCoW (LTI ATS)

### ✅ Must Have (Debe tener - imprescindibles para el MVP)

Estas funcionalidades son el núcleo del producto mínimo viable (MVP).

- **US01**: Como reclutador, quiero crear una nueva vacante y publicarla en portales.
- **US02**: Como reclutador, quiero ver y filtrar candidatos por criterios.
- **US05**: Como manager, quiero revisar candidatos y dejar feedback.
- **US07**: Como candidato, quiero aplicar fácilmente a una vacante.
- **US08**: Como candidato, quiero ver el estado actual de mi postulación.
- **US10**: Como administrador, quiero invitar nuevos miembros y asignar roles.
- **US13**: Como sistema, necesito filtrar candidatos automáticamente.

⸻

### 🟡 Should Have (Debería tener - importantes pero no críticas para el MVP)

Estas funcionalidades mejoran la experiencia general y deberían llegar poco después del MVP.

- **US03**: Como reclutador, quiero que el sistema proponga horarios de entrevista automáticamente.
- **US04**: Como reclutador, quiero dejar observaciones internas sobre un candidato.
- **US06**: Como manager, quiero ver el estado de cada vacante y los procesos activos.
- **US09**: Como candidato, quiero confirmar la propuesta de entrevista o sugerir cambios.
- **US12**: Como administrador, quiero ver reportes sobre el rendimiento del equipo.

⸻

### 🔵 Could Have (Podría tener - deseables si hay tiempo y recursos)

Se implementarán solo si hay disponibilidad de tiempo/equipo tras cubrir las prioridades mayores.

- **US11**: Como administrador, quiero configurar los canales de publicación externos.
- **US14**: Como sistema, quiero proponer horarios óptimos de entrevista según disponibilidad.

⸻

### 🔴 Won’t Have (for now) (No tendrá por ahora)

No se consideran para la primera versión. Serán evaluadas en futuras iteraciones del producto.

- (No hay historias descartadas por ahora, pero funcionalidades como benchmarking o integraciones con ERPs/CRMs podrían entrar aquí más adelante.)

⸻

## 📊 Prioridad de Historias de Usuario – WSJF (LTI ATS)

### 🔍 Fórmula

WSJF = (Valor de Negocio + Urgencia + Reducción de Riesgo) / Tamaño del Trabajo

Valores utilizados en escala relativa (Fibonacci): 1, 2, 3, 5, 8, 13

⸻

### 🏅 Historias Ordenadas por WSJF Score

| Prioridad | ID    | Historia                                                                 | Valor Negocio | Urgencia | Reducción Riesgo | Tamaño | WSJF |
|-----------|-------|--------------------------------------------------------------------------|----------------|----------|-------------------|--------|------|
| 1         | US05  | Revisar candidatos y dejar feedback                                      | 9              | 6        | 6                 | 3      | 7.00 |
| 2         | US01  | Crear y publicar una vacante                                             | 10             | 10       | 8                 | 5      | 5.60 |
| 3         | US08  | Ver el estado de mi candidatura                                          | 6              | 6        | 4                 | 3      | 5.33 |
| 4         | US02  | Ver y filtrar candidatos por criterios                                   | 9              | 8        | 7                 | 5      | 4.80 |
| 5         | US04  | Comentarios internos colaborativos                                       | 6              | 4        | 5                 | 3      | 5.00 |
| 6         | US07  | Aplicar fácilmente a una vacante                                         | 10             | 10       | 5                 | 5      | 5.00 |
| 7         | US09  | Confirmar entrevista propuesta                                           | 6              | 4        | 4                 | 3      | 4.67 |
| 8         | US10  | Invitar nuevos usuarios y asignar roles                                  | 5              | 7        | 6                 | 5      | 3.60 |
| 9         | US06  | Ver el estado general de la vacante                                      | 6              | 5        | 5                 | 5      | 3.20 |
| 10        | US13  | Filtrado automático de candidatos por IA                                 | 9              | 7        | 9                 | 8      | 3.13 |
| 11        | US03  | Propuesta automática de horarios de entrevistas                          | 7              | 5        | 6                 | 8      | 2.25 |
| 12        | US11  | Configurar canales de publicación externos                               | 4              | 3        | 4                 | 5      | 2.20 |
| 13        | US12  | Reportes de rendimiento del equipo                                       | 5              | 4        | 5                 | 8      | 1.75 |
| 14        | US14  | Proponer horarios óptimos de entrevista (algoritmo avanzado)            | 6              | 4        | 6                 | 13     | 1.23 |

⸻

### 🟢 Recomendación para MVP Inicial (Top 5 WSJF)

1. US05 – Revisar candidatos y dejar feedback
2. US01 – Crear y publicar una vacante
3. US08 – Ver el estado de mi candidatura
4. US02 – Ver y filtrar candidatos por criterios
5. US04 – Comentarios internos colaborativos

⸻

## 📦 Product Backlog – LTI ATS (priorizado por WSJF)

### 🎯 Épicas

- **EP01 - Gestión de Vacantes**
- **EP02 - Gestión de Candidatos**
- **EP03 - Colaboración y Feedback**
- **EP04 - Experiencia del Candidato**
- **EP05 - Administración del Sistema**
- **EP06 - Automatización e IA**

---

### 🔝 Prioridad Alta (Top WSJF)

#### ✅ US05 – Revisar candidatos y dejar feedback

- **Descripción**: Como manager, quiero revisar los perfiles de los candidatos y dejar comentarios, para tomar decisiones colaborativas.
- **Prioridad**: WSJF 7.00
- **Tipo**: Feature
- **Épica**: `EP03 - Colaboración y Feedback`

---

#### ✅ US01 – Crear y publicar una vacante

- **Descripción**: Como reclutador, quiero crear una nueva vacante y publicarla en varios portales desde un solo lugar.
- **Prioridad**: WSJF 5.60
- **Tipo**: Feature
- **Épica**: `EP01 - Gestión de Vacantes`

---

#### ✅ US08 – Ver el estado de mi candidatura

- **Descripción**: Como candidato, quiero consultar el estado de mis postulaciones para saber si sigo en el proceso.
- **Prioridad**: WSJF 5.33
- **Tipo**: Feature
- **Épica**: `EP04 - Experiencia del Candidato`

---

#### ✅ US02 – Ver y filtrar candidatos por criterios

- **Descripción**: Como reclutador, quiero aplicar filtros para encontrar candidatos relevantes de manera rápida.
- **Prioridad**: WSJF 4.80
- **Tipo**: Feature
- **Épica**: `EP02 - Gestión de Candidatos`

---

#### ✅ US04 – Comentarios internos colaborativos

- **Descripción**: Como reclutador, quiero dejar notas internas sobre los candidatos para que todo el equipo esté alineado.
- **Prioridad**: WSJF 5.00
- **Tipo**: Feature
- **Épica**: `EP03 - Colaboración y Feedback`

---

#### ✅ US07 – Aplicar fácilmente a una vacante

- **Descripción**: Como candidato, quiero postularme fácilmente usando mi CV o perfil de LinkedIn.
- **Prioridad**: WSJF 5.00
- **Tipo**: Feature
- **Épica**: `EP04 - Experiencia del Candidato`

---

#### ✅ US09 – Confirmar propuesta de entrevista

- **Descripción**: Como candidato, quiero confirmar el horario de la entrevista sugerida por el sistema.
- **Prioridad**: WSJF 4.67
- **Tipo**: Feature
- **Épica**: `EP04 - Experiencia del Candidato`

---

### 🔄 Prioridad Media

#### 🔄 US10 – Invitar nuevos usuarios y asignar roles

- **Descripción**: Como administrador, quiero poder invitar a miembros del equipo y asignarles roles.
- **Prioridad**: WSJF 3.60
- **Tipo**: Feature
- **Épica**: `EP05 - Administración del Sistema`

---

#### 🔄 US06 – Ver estado general del proceso de vacante

- **Descripción**: Como manager, quiero tener una visión clara del estado general del proceso de selección.
- **Prioridad**: WSJF 3.20
- **Tipo**: Feature
- **Épica**: `EP01 - Gestión de Vacantes`

---

#### 🔄 US13 – Filtrado automático con IA

- **Descripción**: Como sistema, necesito filtrar automáticamente candidatos según criterios definidos usando IA.
- **Prioridad**: WSJF 3.13
- **Tipo**: Technical / IA
- **Épica**: `EP06 - Automatización e IA`

---

### 🔽 Prioridad Baja

#### 🔽 US03 – Propuesta automática de entrevistas

- **Descripción**: Como reclutador, quiero que el sistema proponga horarios automáticamente según disponibilidad.
- **Prioridad**: WSJF 2.25
- **Tipo**: Feature
- **Épica**: `EP06 - Automatización e IA`

---

#### 🔽 US11 – Configurar canales externos de publicación

- **Descripción**: Como administrador, quiero definir en qué portales se publican las vacantes.
- **Prioridad**: WSJF 2.20
- **Tipo**: Feature
- **Épica**: `EP05 - Administración del Sistema`

---

#### 🔽 US12 – Acceder a reportes y métricas

- **Descripción**: Como administrador, quiero tener visibilidad de métricas clave del proceso de contratación.
- **Prioridad**: WSJF 1.75
- **Tipo**: Feature
- **Épica**: `EP05 - Administración del Sistema`

---

#### 🔽 US14 – Proponer horarios óptimos con IA (versión avanzada)

- **Descripción**: Como sistema, quiero usar IA avanzada para proponer los mejores horarios posibles de entrevista.
- **Prioridad**: WSJF 1.23
- **Tipo**: Technical / IA
- **Épica**: `EP06 - Automatización e IA`
