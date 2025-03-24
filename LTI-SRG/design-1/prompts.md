# Prompt para Claude utilizando el modelo 3.7 para hacer meta prompting

Eres un prompt enginnering, utilizando todas las buenas praticas del prompting, construye uno con las siguientes instrucciones "LTI es una startup que quiere desarrollar el ATS (Applicant-Tracking System) del futuro.

Todavía no hay nada creado, así que toca ponerse el gorro de product manager y definir esas funcionalidades clave que harán brillar a LTI por encima de los competidores: aumentar la eficiencia para los departamentos de HR, mejorar la colaboración en tiempo real entre reclutadores y managers, automatizaciones, asistencia de IA en diversas tareas...es el momento de hacer brainstorming, investigar cuáles pueden ser las claves del éxito, y dejarlo plasmado para el resto del equipo.

Tu misión es diseñar la primera versión del sistema, entregando los siguientes artefactos:

Descripción breve del software LTI, valor añadido y ventajas competitivas. Explicación de las funciones principales. Añadir un diagrama Lean Canvas para entender el modelo de negocio
Descripción de los 3 casos de uso principales, con el diagrama asociado a cada uno
Modelo de datos que cubra entidades, atributos (nombre y tipo) y relaciones
Diseño del sistema a alto nivel, tanto explicado como diagrama adjunto
Diagrama C4 que llegue en profundidad a uno de los componentes del sistema, el que prefieras"

Documenta todo en un único documento markdown (.md) y establece una estructura ordenada para los diagramas de la solución.

# Prompt para Cursor utilizando Claude 3.7 y el modo agent

## Contexto y Objetivo
Eres un consultor experto en producto para LTI, una startup que busca revolucionar el mercado de los sistemas de seguimiento de candidatos (ATS). Tu tarea es diseñar la primera versión de un ATS innovador que destaque frente a la competencia. Debes pensar como un Product Manager experimentado, identificando las funcionalidades clave que aumentarán la eficiencia en RRHH, mejorarán la colaboración en tiempo real, implementarán automatizaciones efectivas y aprovecharán la IA para optimizar los procesos de reclutamiento.

## Entregables Esperados
Debes proporcionar los siguientes artefactos con un alto nivel de detalle y profesionalidad:

1. **Concepto del Producto**:
   - Descripción concisa del software LTI ATS (máximo 250 palabras)
   - Propuesta de valor única y ventajas competitivas claramente definidas
   - Explicación detallada de 4-6 funcionalidades principales
   - Lean Canvas completo que cubra los 9 elementos clave del modelo de negocio

2. **Análisis de Casos de Uso**:
   - Descripción narrativa de los 3 casos de uso principales
   - Para cada caso, incluye:
     * Actores involucrados
     * Precondiciones
     * Flujo principal paso a paso
     * Flujos alternativos
     * Postcondiciones
   - Diagrama UML de casos de uso para cada escenario

3. **Modelo de Datos**:
   - Identificación de todas las entidades principales del sistema
   - Lista completa de atributos para cada entidad (nombre y tipo de dato)
   - Descripción de las relaciones entre entidades (cardinalidad, dependencias)
   - Diagrama ERD (Entity-Relationship Diagram) normalizado

4. **Arquitectura del Sistema**:
   - Explicación narrativa de la arquitectura de alto nivel
   - Justificación de las decisiones arquitectónicas
   - Tecnologías recomendadas con razonamiento
   - Diagrama arquitectónico que muestre componentes, interfaces y flujos de datos

5. **Diagrama C4**:
   - Nivel 1: Diagrama de contexto del sistema
   - Nivel 2: Diagrama de contenedores
   - Nivel 3: Diagrama de componentes
   - Nivel 4: Diagrama de código para uno de los componentes críticos a tu elección (preferiblemente el más innovador o diferencial)

## Formato y Documentación
- **Documento único**: Entrega toda la documentación en un único archivo Markdown (.md) bien estructurado
- **Estructura del documento**:
  * Incluye una tabla de contenidos con enlaces a las diferentes secciones
  * Utiliza encabezados jerárquicos (H1, H2, H3, etc.) para organizar la información
  * Aplica formato Markdown adecuado (negritas, cursivas, listas, tablas, etc.)
- **Organización de diagramas**:
  * Crea referencias en el documento principal a los diagramas
  * Especifica que los diagramas deben almacenarse en carpetas según su tipo:
    - `/diagramas/casos-de-uso/` para los diagramas UML de casos de uso
    - `/diagramas/modelo-datos/` para el diagrama ERD
    - `/diagramas/arquitectura/` para los diagramas arquitectónicos
    - `/diagramas/c4/` para los diferentes niveles del diagrama C4
  * Indica nombres descriptivos para cada archivo de diagrama (ej: `caso-uso-reclutamiento.png`)

## Directrices de Diseño
- **Innovación**: Prioriza características que no existan en los ATS tradicionales
- **Eficiencia**: Enfócate en reducir pasos manuales y automatizar tareas repetitivas
- **Colaboración**: Diseña para facilitar la comunicación entre equipos de RRHH y managers
- **IA**: Integra capacidades de IA que vayan más allá del simple filtrado de CV
- **Escalabilidad**: Considera cómo el sistema crecerá con el tiempo
- **Experiencia de usuario**: Prioriza la usabilidad tanto para reclutadores como para candidatos

## Enfoque Metodológico
Antes de comenzar el diseño, analiza:
1. Debilidades de los ATS actuales en el mercado
2. Necesidades no satisfechas de los departamentos de RRHH
3. Tendencias tecnológicas emergentes en el sector de reclutamiento
4. Puntos de fricción habituales en los procesos de contratación

A partir de este análisis, diseña un sistema que realmente transforme la experiencia tanto para reclutadores como para candidatos, creando un producto verdaderamente diferencial en el mercado.