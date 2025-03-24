
# 📄 Documentación MVP de HawkeyeHire

Este prompt está diseñado para generar una documentación técnica completa y estructurada del sistema de reclutamiento basado en IA llamado **HawkeyeHire**. Se orienta a equipos ágiles que desarrollan un MVP con enfoque en claridad, jerarquía funcional y especificaciones técnicas detalladas.

---

## ✅ Instrucciones Generales

**Actúa como**:  
Un equipo de profesionales multidisciplinarios (Product Manager, Business Analyst, Technical Lead, Developer, Scrum Master), cada uno con roles definidos para cada sección del documento.

**Objetivo**:  
Generar documentación de implementación detallada en base al archivo fuente PRD que se te proporciono que sirva como guía de desarrollo para el MVP del sistema HawkeyeHire.

**Formato de salida**:  
Guardar el resultado final en `UserStories-RCB.md`.

**Incluir en la documentación**:
- Estructura clara: Épica > Historia de Usuario > Tarea
- Diagramas Mermaid para secuencia, Gantt, etc.
- Tablas ASCII para backlogs y esfuerzo estimado

---

## 🧩 Tabla de Contenidos

1. Visión General del Proyecto  
2. Épicas  
3. Historias de Usuario  
4. Product Backlog  
5. Sprint Backlog  
6. Detalle Técnico de las Tareas T-01 y T-02  
7. Estimación de Esfuerzo  
8. Resultado Esperado

---

## 🧠 Contexto y Roles por Sección

### 1. Visión General del Proyecto  
**Rol**: Product Manager visionario en soluciones de reclutamiento con IA  
_Incluir_: Breve introducción sobre el objetivo del MVP

---

### 2. Épicas  
**Rol**: Senior Product Manager con experiencia en software empresarial y reclutamiento  
_Definir cada épica con_:  
- Epic ID: E-XX  
- Título  
- Descripción  
- Valor de negocio  

---

### 3. Historias de Usuario  
**Rol**: Analista de Negocios Ágil especializado en redacción de historias  
_Formato_:  
- User Story ID: US-XX  
- Título  
- Referencia al Epic ID  
- Descripción  
- "Como [rol], quiero [característica], para que [beneficio]"

---

### 4. Product Backlog  
**Rol**: Product Owner experto en priorización MoSCoW  
_Tablas_:  
```  
| Epic ID | User Story ID | Task ID | Descripción | Prioridad | Tamaño Camiseta |
|---------|---------------|---------|-------------|-----------|------------------|
| E-01    |               |         | Título Épica | Must      |                  |
| E-01    | US-01         |         | Historia 1   | Must      | L                |
| E-01    | US-01         | T-01    | Tarea 1      | Must      | S                |
| E-01    | US-01         | T-02    | Tarea 2      | Must      | XS               |
```

---

### 5. Sprint Backlog  
**Rol**: Líder Técnico  
- Seleccionar una función clave (ej. "Carga y análisis de CVs")  
- Crear 4 tareas pequeñas (2 Frontend, 2 Backend)  
- Incluir tabla con:  
```  
| Task ID | Título Corto          | Capa     | Asignado | Story Points | Esfuerzo     |
|---------|------------------------|----------|----------|--------------|--------------|
| T-01    | Crear componente Upload| Frontend | Miguel   | 2            | ~4h          |
| T-02    | Endpoint de Upload     | Backend  | Sofia    | 3            | ~8h          |
```

- Agregar un diagrama Mermaid Gantt

---

### 6. Detalle de Tareas T-01 y T-02  
**Rol**: Desarrollador Full-stack Senior  
_Sólo documentación técnica, sin código_

Para cada tarea, incluir:  
- Diagrama Mermaid de secuencia  
- Descripción  
- Definición de hecho  
- Dependencias  
- Detalles según la capa (Frontend/Backend)  
- Estrategia de testing: Unitario, Integración, E2E, Edge Cases

---

### 7. Estimación de Esfuerzo  
**Rol**: Scrum Master  
- Estimar con secuencia Fibonacci (1, 2, 3, 5, 8, 13, 21)  
- Tabla con justificación:  
```  
| Task ID | Story Points | Justificación           |
|---------|--------------|--------------------------|
| T-01    | 2            | Breve razón de la estimación |
```  
- Explicar lo que representa cada punto Fibonacci  
- Incluir capacidad total del sprint

---

### 8. Resultado Esperado  
Describir el resultado funcional del MVP tras implementar las tareas.

--
## conclusiones

Crear GPTS para elaborar las tareas e indicarle roles o instrucciones especificas facilita el trabajo, se hizo todo con chatGpt 4.5