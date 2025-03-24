# UserStories-JM

## 1. Historial de Prompts (Conversaciones y Resultados)

### Prompt 1 - Generar User Stories a partir de la necesidad general
> "Eres un Scrum Master experto en metodologías ágiles, con amplia experiencia liderando equipos técnicos en el desarrollo de software, especializado en crear User Stories efectivas, organizar backlogs claros y facilitar la generación precisa de tickets técnicos para proyectos innovadores utilizando inteligencia artificial. Crea dos User Stories basadas en una aplicación que entrevista candidatos usando IA. Que tengan claridad en el rol, funcionalidad esperada y beneficio para el usuario."

**Resultado:**
Se generaron dos historias claras que sirvieron como base para el backlog. Este prompt fue útil porque partió del objetivo general del ejercicio y ayudó a estructurar bien las funcionalidades esperadas.

---

### Prompt 2 - Refinamiento de User Stories para cumplir estándares
> "¿Podés revisar estas User Stories para asegurarte de que tengan rol, necesidad y justificación, y estén alineadas a buenas prácticas?"

**Resultado:**
Las historias fueron pulidas con lenguaje más técnico y alineadas con el estándar INVEST. Este prompt ayudó a afinar detalles que al principio pasamos por alto.

---

### Prompt 3 - Generación del Backlog priorizado
> "Ahora, generá un Backlog priorizado a partir de estas User Stories, usando MoSCoW como metodología efectiva para priorizar funcionalidades."

**Resultado:**
Se elaboró un backlog en orden de prioridad clara. Este fue el prompt más valioso, ya que permitió transformar la visión general en pasos concretos y accionables.

---

### Prompt 4 - Creación de tickets técnicos desde una User Story
> "A partir de la User Story 1 generá al menos 3 tickets técnicos, (Objetivo, Tareas Técnicas, Responsable, Dependencias, Estimación, Prioridad, Estado) con tareas específicas que el equipo de desarrollo pueda implementar."

**Resultado:**
Se generaron tareas claras, técnicas y factibles para implementar desde frontend y backend. Este prompt facilitó la planificación futura con claridad.

---

### Prompt 5 - Estimación del esfuerzo de los tickets
> "Estimá el esfuerzo de trabajo de cada ticket con metodología de tallas de camiseta y justificación de por qué esa estimación es adecuada."

**Resultado:**
Este paso fue clave para aplicar criterios reales de planificación y ejecución.

---

## 2. Resultado del Ejercicio

### User Story 1
**Como** Reclutador Técnico  
**Quiero** acceder a un panel donde pueda visualizar los resultados de entrevistas hechas por la IA  
**Para** tomar decisiones de contratación más informadas y rápidas.

### User Story 2  
**Como** Candidato a un cargo  
**Quiero** hacer entrevistas técnicas automatizadas desde mi celular  
**Para** poder postularme a empresas sin depender de horarios específicos.

---

### Backlog Priorizado (Método MoSCoW)

1. [MUST] Implementar el panel para reclutadores (User Story 1)
2. [MUST] Crear experiencia móvil para entrevistas (User Story 2)
3. [SHOULD] Agregar test de personalidad con IA
4. [COULD] Personalización de avatares en entrevistas
5. [WON'T] Integración con redes sociales en esta fase

---

## 🎟️ Tickets Técnicos (Formato Mejorado)

### 📌 Ticket 1: Crear componente Frontend para Panel de Reclutador

- **ID:** TKT-101
    
- **Objetivo:**  
    Desarrollar la interfaz visual que permitirá a los reclutadores revisar resultados y detalles de entrevistas.
    
- **Tareas Técnicas:**
    
    - Crear mockup inicial de UI
        
    - Implementar maquetación con HTML/CSS/Tailwind
        
    - Conectar con backend vía API REST
        
- **Responsable:** Equipo Frontend
    
- **Dependencias:** Diseño aprobado por equipo UX
    
- **Estimación:** 🟡 5 puntos (Alta complejidad)
    
- **Prioridad:** 🔴 Alta
    
- **Estado:** 🕒 Por hacer
    

---

### 📌 Ticket 2: Diseñar API REST para Consulta de Entrevistas Almacenadas

- **ID:** TKT-102
    
- **Objetivo:**  
    Construir endpoints REST seguros y eficientes que permitan obtener resultados y métricas clave de entrevistas guardadas.
    
- **Tareas Técnicas:**
    
    - Definir estructura del JSON de respuestas
        
    - Implementar endpoints GET y POST (CRUD básico)
        
    - Añadir autenticación JWT para seguridad
        
- **Responsable:** Equipo Backend
    
- **Dependencias:** Base de datos configurada
    
- **Estimación:** 🟢 3 puntos (Media complejidad)
    
- **Prioridad:** 🔴 Alta
    
- **Estado:** 🕒 Por hacer
    

---

### 📌 Ticket 3: Adaptar Diseño Móvil para Candidatos con Test Automatizados

- **ID:** TKT-103
    
- **Objetivo:**  
    Asegurar una experiencia óptima y fluida para candidatos en entrevistas técnicas desde dispositivos móviles.
    
- **Tareas Técnicas:**
    
    - Realizar diseño responsive para teléfonos y tabletas
        
    - Integrar componentes de test automático interactivo
        
    - Optimizar rendimiento y tiempos de carga
        
- **Responsable:** Equipo Frontend / UX
    
- **Dependencias:** Integración con módulo IA
    
- **Estimación:** 🟠 8 puntos (Muy alta complejidad)
    
- **Prioridad:** 🟡 Media-Alta
    
- **Estado:** 🕒 Por hacer

---

### Estimación de Esfuerzo

| Ticket                      | Estimación | Justificación                  |
|----------------------------|------------|-------------------------------|
| Componente frontend panel  | M (Media)  | Requiere diseño e integración |
| API REST entrevistas       | L (Grande) | Maneja lógica y autenticación |
| Diseño móvil entrevistas   | XL (Extra) | Incluye interfaz + test IA    |

---

## 3. Conclusión del Trabajo

Este ejercicio me permitió aplicar de forma muy clara lo aprendido sobre metodologías ágiles. Entender cómo se estructuran y refinan las User Stories, priorizar un backlog realista y generar tickets que aterrizan técnicamente cada funcionalidad fue clave. 

Además, todo este proceso es de gran importancia desde los procesos actuales que he empezado a implementar en mi empresa **Nexo Digital**, ya que recientemente comenzamos a adoptar metodologías ágiles como Scrum, definir indicadores y organizar mejor nuestros sprints semanales. La falta de User Stories bien escritas generó desorden y tareas mal planificadas, por lo cual este módulo me dio herramientas prácticas y efectivas que ya empezamos a aplicar con el equipo para mejorar como empresa tecnológica y de formación.

---

## 4. Resumen Profesional (para entregar como informe PDF)

- Se redactaron dos User Stories alineadas con la metodología INVEST
- Se generó un backlog usando priorización MoSCoW
- Se crearon tres tickets técnicos derivados de una historia seleccionada
- Se estimó esfuerzo por tallas de camiseta y se justificó cada caso
- Se documentó todo el proceso con prompts usados y conclusiones
- El aprendizaje se aplicará en Nexo Digital a nivel de planificación y SCRUM

