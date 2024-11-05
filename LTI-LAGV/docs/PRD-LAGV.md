
# Documento de Requisitos del Producto (PRD)
## Applicant-Tracking System (ATS) - LTI

---

## 1. Resumen Ejecutivo

LTI ATS es una plataforma de seguimiento de candidatos que mejora los procesos de reclutamiento mediante la integración de funciones de colaboración en tiempo real y tecnologías de inteligencia artificial (IA). Este sistema está diseñado para agilizar la clasificación de CVs, evaluar automáticamente a los candidatos, y facilitar la comunicación instantánea entre reclutadores y managers a través de un chat en vivo.

## 2. Objetivos del Proyecto

1. Automatizar tareas repetitivas y administrativas en el proceso de reclutamiento.
2. Facilitar la colaboración en tiempo real entre los equipos de reclutamiento y los managers.
3. Optimizar el proceso de selección mediante la clasificación automática de CVs.
4. Proveer herramientas de evaluación automatizada para mejorar la toma de decisiones.
5. Incorporar funciones de IA para personalizar y hacer más eficiente el reclutamiento.

## 3. Alcance del Producto

El sistema ATS cubrirá las siguientes funciones principales:
- Clasificación automática de CVs.
- Evaluación automatizada de candidatos.
- Chat en vivo entre reclutadores y managers para una colaboración más fluida.
- Generación de recordatorios automáticos y respuestas a candidatos.
- Análisis de tono en respuestas de entrevistas.

## 4. Requisitos Funcionales

1. **Clasificación Automática de CVs**
    - Filtrar y clasificar CVs con base en criterios predefinidos.
    - Integración con IA para mejorar la precisión de las clasificaciones.

2. **Evaluación Automatizada de Candidatos**
    - Permitir a los reclutadores y managers realizar evaluaciones automatizadas en función de las habilidades y la experiencia.
    - Generación de informes automáticos de evaluación.

3. **Chat en Vivo**
    - Comunicación en tiempo real entre reclutadores y managers.
    - Notificaciones automáticas para nuevos mensajes y eventos importantes.

4. **Automatización de Respuestas y Recordatorios**
    - Envío de mensajes automáticos a los candidatos en diferentes etapas del proceso de selección.
    - Creación de recordatorios automáticos para entrevistas y evaluaciones.

5. **Análisis de Tono**
    - Uso de IA para evaluar el tono y la receptividad en las respuestas de los candidatos.

## 5. Requisitos No Funcionales

- **Rendimiento**: El sistema debe responder en menos de 2 segundos para las consultas de CVs y evaluaciones.
- **Escalabilidad**: Capacidad de manejar una base de datos de hasta 1 millón de registros sin degradación en el rendimiento.
- **Seguridad**: Autenticación y autorización para proteger los datos sensibles.
- **Compatibilidad**: Optimización para los navegadores modernos y móviles.
- **Disponibilidad**: Uptime del 99.9% durante el horario laboral.

## 6. Casos de Uso

1. **Caso de Uso 1: Clasificación Automática de CVs**
    - Actores: Reclutador, Sistema de IA.
    - Descripción: El sistema analiza y clasifica los CVs automáticamente basándose en los requisitos del puesto.

2. **Caso de Uso 2: Evaluación Automatizada de Candidatos**
    - Actores: Reclutador, Manager, Sistema de IA.
    - Descripción: Permite una evaluación automática de las habilidades de los candidatos y proporciona un informe de adecuación.

3. **Caso de Uso 3: Chat en Vivo entre Reclutadores y Managers**
    - Actores: Reclutador, Manager.
    - Descripción: Permite la comunicación en tiempo real entre reclutadores y managers durante el proceso de selección.

## 7. Especificaciones de Diseño

- **Diagrama C4 de Componentes**: La arquitectura estará dividida en componentes principales que incluyen módulos para IA, bases de datos, gestión de usuarios y funcionalidades de chat.
- **Modelo de Datos**: Tablas de entidades para candidatos, puestos de trabajo, usuarios (reclutadores y managers), y registros de chat.

## 8. Criterios de Aceptación

1. La clasificación automática debe procesar CVs de forma precisa con un 90% de coincidencia.
2. El chat debe ser funcional y sin retrasos perceptibles.
3. Las evaluaciones automatizadas deben generarse en un plazo de 2 segundos.
4. Los recordatorios y respuestas automáticas deben activarse según las reglas de flujo establecidas.

## 9. Consideraciones Técnicas

- **Lenguajes y Frameworks**: Basado en el uso de Angular y tecnologías modernas para IA y procesamiento en tiempo real.
- **Tecnologías Open Source**: Implementación de herramientas open-source para el análisis de CVs y procesamiento de datos.
- **Almacenamiento en la Nube**: Para asegurar la escalabilidad y disponibilidad.

---

Este PRD complementa la documentación inicial, proporcionando una base sólida para el desarrollo y una referencia clara para los equipos de desarrollo y producto.
