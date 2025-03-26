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

**US01** - Crear y publicar una vacante

Como reclutador, quiero crear una nueva vacante y publicarla en múltiples portales, para recibir candidatos lo antes posible.

**US02** - Ver y filtrar candidatos por vacante

Como reclutador, quiero ver la lista de candidatos aplicados a una vacante, y filtrarlos por experiencia, palabras clave o skills, para enfocarme en los más adecuados.

**US03** - Programar entrevistas automáticamente

Como reclutador, quiero que el sistema proponga horarios de entrevista automáticamente según la disponibilidad, para ahorrar tiempo y evitar conflictos.

**US04** - Dejar comentarios sobre un candidato

Como reclutador, quiero anotar observaciones internas sobre un candidato, para compartirlas con el equipo y tomar decisiones en conjunto.

⸻

### 🧑‍💼 Manager de contratación

**US05** - Revisar candidatos y dejar feedback

Como manager, quiero ver los perfiles de candidatos seleccionados y añadir feedback colaborativo, para facilitar la elección del mejor perfil.

**US06** - Ver el estado del proceso de selección

Como manager, quiero tener una vista clara del estado de cada vacante, para entender en qué etapa está cada candidato.

⸻

### 🙋 Candidato

**US07** - Aplicar a una vacante

Como candidato, quiero aplicar fácilmente a una vacante con mi CV y LinkedIn, para postularme sin fricciones.

**US08** - Ver el estado de mi candidatura

Como candidato, quiero ver el estado actual de mi postulación, para saber si sigo en el proceso o fui descartado.

**US09** - Confirmar entrevista sugerida

Como candidato, quiero recibir una notificación con la propuesta de horario de entrevista y poder confirmarla o sugerir cambios, para coordinar de manera cómoda.

⸻

### 🛠️ Administrador de empresa

**US10** - Invitar nuevos usuarios

Como administrador de empresa, quiero invitar nuevos miembros al sistema, asignándoles roles, para gestionar mi equipo de reclutamiento.

**US11** - Configurar canales de publicación

Como administrador, quiero configurar qué portales de empleo se conectan con LTI, para publicar vacantes desde una única plataforma.

**US12** - Acceder a reportes y estadísticas

Como administrador, quiero ver métricas como tiempo promedio de contratación o número de entrevistas, para analizar el rendimiento del equipo de RRHH.

⸻

### 🤖 Sistema / Automatización / IA

**US13** - Filtrar candidatos automáticamente

Como sistema, necesito analizar los CVs recibidos y filtrarlos por relevancia, para presentar primero los candidatos con mejor match.

**US14** - Proponer horario óptimo de entrevista

Como sistema, necesito calcular un horario óptimo de entrevista según disponibilidad de partes involucradas, para evitar solapamientos y optimizar el tiempo.

⸻

## 🧭 Prioridad de Historias de Usuario – MoSCoW (LTI MMA)

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

## 📊 Prioridad de Historias de Usuario – WSJF (LTI MMA)

### 🔍 Fórmula

WSJF = (Valor de Negocio + Urgencia + Reducción de Riesgo) / Tamaño del Trabajo

Valores utilizados en escala relativa (Fibonacci): 1, 2, 3, 5, 8, 13

⸻

### 🏅 Historias Ordenadas por WSJF Score

```markdown
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
````

⸻

### 🟢 Recomendación para MVP Inicial (Top 5 WSJF)

1. **US05** – Revisar candidatos y dejar feedback
2. **US01** – Crear y publicar una vacante
3. **US08** – Ver el estado de mi candidatura
4. **US02** – Ver y filtrar candidatos por criterios
5. **US04** – Comentarios internos colaborativos

⸻

## 📦 Product Backlog – LTI MMA (priorizado por WSJF)

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

---

## 📦 Product Backlog – LTI MMA (priorizado por MoSCoW)

### 🎯 Épicas

- **EP01 - Gestión de Vacantes**
- **EP02 - Gestión de Candidatos**
- **EP03 - Colaboración y Feedback**
- **EP04 - Experiencia del Candidato**
- **EP05 - Administración del Sistema**
- **EP06 - Automatización e IA**

---

### ✅ Must Have (Debe tener - MVP)

#### US01 – Crear y publicar una vacante

- **Descripción**: Como reclutador, quiero crear una nueva vacante y publicarla en varios portales desde un solo lugar.
- **Tipo**: Feature
- **Épica**: `EP01 - Gestión de Vacantes`

---

#### US02 – Ver y filtrar candidatos por criterios

- **Descripción**: Como reclutador, quiero aplicar filtros para encontrar candidatos relevantes de manera rápida.
- **Tipo**: Feature
- **Épica**: `EP02 - Gestión de Candidatos`

---

#### US05 – Revisar candidatos y dejar feedback

- **Descripción**: Como manager, quiero revisar los perfiles de los candidatos y dejar comentarios, para tomar decisiones colaborativas.
- **Tipo**: Feature
- **Épica**: `EP03 - Colaboración y Feedback`

---

#### US07 – Aplicar fácilmente a una vacante

- **Descripción**: Como candidato, quiero postularme fácilmente usando mi CV o perfil de LinkedIn.
- **Tipo**: Feature
- **Épica**: `EP04 - Experiencia del Candidato`

---

#### US08 – Ver el estado de mi candidatura

- **Descripción**: Como candidato, quiero consultar el estado de mis postulaciones para saber si sigo en el proceso.
- **Tipo**: Feature
- **Épica**: `EP04 - Experiencia del Candidato`

---

#### US10 – Invitar nuevos usuarios y asignar roles

- **Descripción**: Como administrador, quiero poder invitar a miembros del equipo y asignarles roles.
- **Tipo**: Feature
- **Épica**: `EP05 - Administración del Sistema`

---

#### US13 – Filtrado automático con IA

- **Descripción**: Como sistema, necesito filtrar automáticamente candidatos según criterios definidos usando IA.
- **Tipo**: Technical / IA
- **Épica**: `EP06 - Automatización e IA`

---

### 🟡 Should Have (Debería tener - versión posterior al MVP)

#### US03 – Propuesta automática de entrevistas

- **Descripción**: Como reclutador, quiero que el sistema proponga horarios automáticamente según disponibilidad.
- **Tipo**: Feature
- **Épica**: `EP06 - Automatización e IA`

---

#### US04 – Comentarios internos colaborativos

- **Descripción**: Como reclutador, quiero dejar notas internas sobre los candidatos para que todo el equipo esté alineado.
- **Tipo**: Feature
- **Épica**: `EP03 - Colaboración y Feedback`

---

#### US06 – Ver estado general del proceso de vacante

- **Descripción**: Como manager, quiero tener una visión clara del estado general del proceso de selección.
- **Tipo**: Feature
- **Épica**: `EP01 - Gestión de Vacantes`

---

#### US09 – Confirmar propuesta de entrevista

- **Descripción**: Como candidato, quiero confirmar el horario de la entrevista sugerida por el sistema.
- **Tipo**: Feature
- **Épica**: `EP04 - Experiencia del Candidato`

---

#### US12 – Acceder a reportes y métricas

- **Descripción**: Como administrador, quiero tener visibilidad de métricas clave del proceso de contratación.
- **Tipo**: Feature
- **Épica**: `EP05 - Administración del Sistema`

---

### 🔵 Could Have (Podría tener - si hay tiempo o recursos)

#### US11 – Configurar canales externos de publicación

- **Descripción**: Como administrador, quiero definir en qué portales se publican las vacantes.
- **Tipo**: Feature
- **Épica**: `EP05 - Administración del Sistema`

---

#### US14 – Proponer horarios óptimos con IA (versión avanzada)

- **Descripción**: Como sistema, quiero usar IA avanzada para proponer los mejores horarios posibles de entrevista.
- **Tipo**: Technical / IA
- **Épica**: `EP06 - Automatización e IA`

---

### 🔴 Won’t Have (for now)

_No se han identificado historias a excluir por ahora._

---

## 📊 Comparativa de Prioridades: WSJF vs MoSCoW – LTI MMA

Acontinuacion comparamos los resultados de priorizar el backlog del sistema LTI utilizando dos técnicas distintas: **WSJF (Weighted Shortest Job First)** y **MoSCoW**.

---

### 🧠 Enfoques metodológicos

```markdown
| Criterio                | WSJF                                      | MoSCoW                                          |
|-------------------------|-------------------------------------------|-------------------------------------------------|
| Basado en...            | Cálculo de valor relativo y coste/tiempo | Clasificación por criticidad funcional          |
| Objetivo principal      | Maximizar valor entregado en el menor tiempo posible | Definir qué es imprescindible en el MVP       |
| Ideal para...           | Equipos con muchas iniciativas en backlog | Proyectos en fases tempranas (MVP, v1)          |
```

---

### 🔍 Diferencias clave entre ambos backlogs

#### 1. Orden de prioridad no coincide

```markdown
| Historia                                | Prioridad en WSJF | Prioridad en MoSCoW |
|----------------------------------------|--------------------|----------------------|
| US05 – Feedback colaborativo           | #1 (WSJF 7.0)      | Must Have           |
| US01 – Crear y publicar vacante        | #2 (WSJF 5.6)      | Must Have           |
| US08 – Estado de candidatura           | #3 (WSJF 5.3)      | Must Have           |
| US13 – Filtrado IA                     | #10 (WSJF 3.13)    | Must Have           |
| US03 – Horarios automáticos            | #11 (WSJF 2.25)    | Should Have         |
| US14 – Horarios óptimos con IA         | #14 (WSJF 1.23)    | Could Have          |
| US12 – Reportes y métricas             | #13 (WSJF 1.75)    | Should Have         |
```

**Análisis**:

- WSJF da prioridad a tareas de **alto valor y bajo coste** (como US05).
- MoSCoW da prioridad a lo que es **funcionalmente imprescindible para el MVP** (como US13), aunque implique mayor esfuerzo.

---

#### 2. Cobertura del MVP

- **MoSCoW** delimita con claridad el MVP: todo lo que es “Must Have” debe estar en la primera versión.
- **WSJF** entrega una cola ordenada, pero no especifica qué historias se deben incluir en el MVP. Requiere una decisión adicional.

---

#### 3. Énfasis en valor inmediato vs. visión estratégica

- **WSJF** prioriza lo que entrega **valor temprano y rápido** (p. ej., feedback, filtros).
- **MoSCoW** prioriza lo que el sistema **necesita para funcionar de forma coherente**, incluso si es más costoso (p. ej., automatización IA básica).

---

### 🏁 Conclusión

```markdown
| Aspecto                  | WSJF                          | MoSCoW                       |
|--------------------------|-------------------------------|------------------------------|
| ¿Define MVP?             | No (requiere decisión externa)| Sí (Must Have es el MVP)     |
| ¿Ordena toda la cola?    | Sí                            | Parcialmente                 |
| ¿Evalúa esfuerzo?        | Sí                            | No                           |
| ¿Fácil para stakeholders?| Más técnico                   | Más comprensible             |
```

---

### ✅ Recomendación

> Utilizar **MoSCoW para definir el alcance del MVP**, y luego aplicar **WSJF para ordenar la implementación dentro del MVP**, maximizando el valor por iteración.

---

## 📦 Backlog Unificado – LTI MMA (WSJF + MoSCoW)

Este backlog muestra todas las historias de usuario de LTI MMA, junto con su prioridad tanto por **WSJF** como por **MoSCoW**, para tener una visión integral de valor vs. necesidad funcional.

---

### 🧩 Leyenda de Épicas

- `EP01 - Gestión de Vacantes`
- `EP02 - Gestión de Candidatos`
- `EP03 - Colaboración y Feedback`
- `EP04 - Experiencia del Candidato`
- `EP05 - Administración del Sistema`
- `EP06 - Automatización e IA`

---

### 🗂️ Backlog Detallado

```markdown
| ID    | Historia                                           | WSJF Score | MoSCoW     | Épica                      |
|-------|----------------------------------------------------|------------|------------|-----------------------------|
| US05  | Revisar candidatos y dejar feedback                | 7.00       | Must Have  | EP03 - Feedback             |
| US01  | Crear y publicar una vacante                       | 5.60       | Must Have  | EP01 - Vacantes             |
| US08  | Ver el estado de mi candidatura                    | 5.33       | Must Have  | EP04 - Experiencia          |
| US02  | Ver y filtrar candidatos                           | 4.80       | Must Have  | EP02 - Candidatos           |
| US04  | Comentarios internos colaborativos                 | 5.00       | Should Have| EP03 - Feedback             |
| US07  | Aplicar a una vacante                              | 5.00       | Must Have  | EP04 - Experiencia          |
| US09  | Confirmar entrevista sugerida                      | 4.67       | Should Have| EP04 - Experiencia          |
| US10  | Invitar nuevos usuarios y roles                    | 3.60       | Must Have  | EP05 - Administración       |
| US06  | Ver estado general de vacantes                     | 3.20       | Should Have| EP01 - Vacantes             |
| US13  | Filtrado automático con IA                         | 3.13       | Must Have  | EP06 - IA                   |
| US03  | Propuesta automática de entrevistas                | 2.25       | Should Have| EP06 - IA                   |
| US11  | Configurar canales de publicación externos         | 2.20       | Could Have | EP05 - Administración       |
| US12  | Reportes y métricas del sistema                    | 1.75       | Should Have| EP05 - Administración       |
| US14  | IA avanzada para horarios óptimos                  | 1.23       | Could Have | EP06 - IA                   |
```

---

### 🔍 Observaciones

- Las historias **US05, US01, US08, US02** aparecen tanto con alta puntuación WSJF como en la categoría **Must Have** de MoSCoW ⇒ ideales para desarrollo temprano.
- **US13 (IA básica)** tiene WSJF medio pero es Must Have por visión estratégica y diferenciación del producto.
- Historias como **US11 y US14** tienen baja puntuación y baja prioridad ⇒ se pueden posponer para fases posteriores.

---

## 🎟️ Ticket: US01 – Crear y publicar una vacante

**Tipo:** Feature  
**Prioridad:** Alta (Must Have / WSJF 5.6)  
**Épica:** EP01 - Gestión de Vacantes  
**Estado:** Por hacer  
**Asignado a:** [A definir]  
**Sprint:** MVP Sprint 1  

---

### 🧠 Descripción

Como **reclutador**, quiero **crear una nueva vacante y publicarla en múltiples portales**, para **recibir candidatos lo antes posible** y gestionar el proceso desde una única plataforma.

---

### ✅ Criterios de Aceptación (AC)

1. ✅ El reclutador puede acceder a una pantalla o modal de “Crear vacante”.
2. ✅ Puede completar los siguientes campos obligatorios: título, descripción, tipo de contrato, ubicación, salario (opcional), área, y nivel de experiencia.
3. ✅ Puede seleccionar los canales externos de publicación (ej: LinkedIn, InfoJobs, Web propia).
4. ✅ Al guardar, la vacante se almacena en la base de datos y se muestra en el listado de vacantes activas.
5. ✅ Si se seleccionaron canales externos, se inicia el proceso de publicación en esos portales vía API.
6. ✅ El sistema muestra un mensaje de éxito o errores de validación al guardar.
7. ✅ La vacante queda editable por parte del reclutador una vez creada.

---

### 🧪 Criterios de Validación Técnica

- Los campos deben ser validados tanto en frontend como backend.
- Las integraciones externas deben estar desacopladas (job async en segundo plano).
- Debe existir un modelo `JobPosting` relacionado con `Company` y `User`.
- Se debe registrar un log del evento de creación de vacante.

---

### 🧱 Tareas Técnicas (sub-tareas sugeridas)

- [ ] Crear endpoint API REST para crear vacantes (`POST /api/vacancies/`)
- [ ] Diseñar formulario en frontend (React/Vue) para capturar datos de la vacante
- [ ] Validar campos requeridos en backend
- [ ] Configurar relación entre `Vacancy`, `Company` y `User`
- [ ] Implementar publicación simulada (mock) en portales externos
- [ ] Añadir pruebas unitarias y de integración
- [ ] Documentar en Swagger/Postman

---

### 🧩 Dependencias

- US10 – Gestión de usuarios y roles (para saber si el usuario tiene permiso de publicar).
- US11 – Configurar canales de publicación (opcional para MVP, pero si no está, usar canal por defecto).

---

### 📎 Recursos útiles

- Diseño UI de formulario (Figma): _[Link si disponible]_
- Docs de API externa para publicar vacantes: _[Link si disponible]_

---

## ⏱️ Estimación de Esfuerzo – US01: Crear y Publicar una Vacante

> Método utilizado: **Fibonacci (adaptado a horas)**  
> Unidad de medida: **Horas estimadas**

---

### 🎟️ Historia de Usuario

**US01 – Crear y publicar una vacante**  
**Como** reclutador  
**Quiero** crear una nueva vacante y publicarla en múltiples portales  
**Para** recibir candidatos lo antes posible y gestionarlo desde un solo lugar.

---

### 📐 Escala Fibonacci (adaptada a horas)

Esta escala se usa para estimar el esfuerzo relativo de tareas en proyectos ágiles, con un rango de horas estimadas para cada punto.

```markdown
| Puntos Fibonacci | Rango de Horas Estimadas | Descripción                                  |
|------------------|---------------------------|----------------------------------------------|
| 1                | 1–2 horas                 | Tarea trivial o configuración mínima         |
| 2                | 2–4 horas                 | Tarea sencilla, bien definida                |
| 3                | 4–6 horas                 | Tarea con lógica intermedia                  |
| 5                | 6–10 horas                | Tarea de jornada completa aproximadamente    |
| 8                | 10–16 horas               | Tarea de hasta 2 días de trabajo             |
| 13               | 16–24 horas               | Tarea compleja, implica varios componentes   |
| 21               | 24–40 horas               | Tarea muy compleja, casi una épica           |
````

> ⚠️ Nota: esta tabla sirve como guía relativa. Las horas pueden ajustarse según la experiencia del equipo y el contexto técnico.

---

### 📋 Subtareas con estimación

```markdown
| Subtarea                                                                 | Puntos Fibonacci | Rango de Horas Estimadas |
|--------------------------------------------------------------------------|------------------|---------------------------|
| Crear endpoint API REST para crear vacantes (`POST /api/vacancies/`)     | 5                | 6–10 h                    |
| Diseñar formulario en frontend para capturar datos                       | 3                | 4–6 h                     |
| Validar campos requeridos en backend                                     | 2                | 2–4 h                     |
| Configurar relación entre `Vacancy`, `Company` y `User`                  | 2                | 2–4 h                     |
| Implementar publicación simulada en portales externos                    | 3                | 4–6 h                     |
| Añadir pruebas unitarias y de integración                                | 5                | 6–10 h                    |
| Documentar en Swagger/Postman                                            | 1                | 1–2 h                     |
````

---

### 🧮 Estimación Total

- **Total puntos**: `21` (equivalente a una tarea compleja)
- **Rango total estimado**: `25–42 horas`
- **Duración estimada**: `3 a 5 jornadas de desarrollo` (dependiendo del perfil)

---

### 👥 Sugerencia de asignación

Este ticket puede dividirse entre:

- 1 desarrollador backend
- 1 desarrollador frontend

**Objetivo**: entregar esta funcionalidad dentro del Sprint 1 del MVP.

---
