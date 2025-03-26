# Documentación de Implementación de LTI ATS

## Tabla de Contenidos
- [1. Historias de Usuario](#1-historias-de-usuario)
  - [1.1 Historia de Usuario: Emparejamiento Inteligente de Candidatos](#11-historia-de-usuario-emparejamiento-inteligente-de-candidatos)
  - [1.2 Historia de Usuario: Colaboración en Tiempo Real](#12-historia-de-usuario-colaboración-en-tiempo-real)
  - [1.3 Historia de Usuario: Automatización del Proceso de Contratación](#13-historia-de-usuario-automatización-del-proceso-de-contratación)
  - [1.4 Historia de Usuario: Experiencia del Candidato](#14-historia-de-usuario-experiencia-del-candidato)
  - [1.5 Historia de Usuario: Análisis Predictivo de Reclutamiento](#15-historia-de-usuario-análisis-predictivo-de-reclutamiento)
- [2. Product Backlog](#2-product-backlog)
  - [2.1 Priorización MoSCoW](#21-priorización-moscow)
  - [2.2 Proceso de Prompt Engineering](#22-proceso-de-prompt-engineering)
- [3. Tickets Técnicos: Historia de Usuario 1](#3-tickets-técnicos-historia-de-usuario-1)
  - [3.1 Implementación del Analizador Semántico de CV](#31-implementación-del-analizador-semántico-de-cv)
  - [3.2 Desarrollo del Motor de Vectorización de Perfiles](#32-desarrollo-del-motor-de-vectorización-de-perfiles)
  - [3.3 Implementación del Algoritmo de Matching Semántico](#33-implementación-del-algoritmo-de-matching-semántico)
  - [3.4 Desarrollo de API para el Servicio de Emparejamiento](#34-desarrollo-de-api-para-el-servicio-de-emparejamiento)
  - [3.5 Creación de Interfaz de Presentación de Resultados](#35-creación-de-interfaz-de-presentación-de-resultados)
- [4. Estimación de Esfuerzo](#4-estimación-de-esfuerzo)
  - [4.1 Metodología de Estimación](#41-metodología-de-estimación)
  - [4.2 Estimaciones por Historia de Usuario](#42-estimaciones-por-historia-de-usuario)
  - [4.3 Tabla Resumen de Estimaciones](#43-tabla-resumen-de-estimaciones)
- [5. Apéndice: Suposiciones](#5-apéndice-suposiciones)

## 1. Historias de Usuario

### 1.1 Historia de Usuario: Emparejamiento Inteligente de Candidatos

**Como** reclutador,  
**Quiero** que el sistema empareje automáticamente candidatos con vacantes utilizando análisis semántico,  
**Para** identificar a los candidatos más adecuados incluso cuando no coinciden exactamente con las palabras clave tradicionales.

**Criterios de Aceptación:**
1. El sistema debe analizar semánticamente los CV y las descripciones de puestos para comprender habilidades, experiencia y potencial.
2. Los resultados deben mostrar una puntuación de compatibilidad multidimensional (habilidades técnicas, habilidades blandas, alineación cultural).
3. El sistema debe proporcionar explicaciones sobre por qué un candidato es una buena coincidencia para la vacante.
4. Los resultados deben ser presentados en una lista ordenada por relevancia con opciones de filtrado adicionales.
5. El sistema debe aprender de las decisiones de contratación pasadas para mejorar futuras recomendaciones.

**Categoría:** IA y Machine Learning

### 1.2 Historia de Usuario: Colaboración en Tiempo Real

**Como** gerente de contratación,  
**Quiero** colaborar en tiempo real con mi equipo durante el proceso de evaluación de candidatos,  
**Para** tomar decisiones de contratación más rápidas y mejor informadas.

**Criterios de Aceptación:**
1. Todos los miembros del equipo deben poder ver y comentar sobre los perfiles de candidatos simultáneamente.
2. Durante las entrevistas, los evaluadores deben poder compartir notas y evaluaciones en tiempo real.
3. El sistema debe agregar automáticamente las evaluaciones individuales y generar un resumen comparativo.
4. Los miembros del equipo que no puedan asistir a entrevistas en vivo deben poder revisar grabaciones con anotaciones.
5. El sistema debe alertar sobre evaluaciones significativamente divergentes y facilitar la discusión para alcanzar consenso.

**Categoría:** Colaboración y Comunicación

### 1.3 Historia de Usuario: Automatización del Proceso de Contratación

**Como** reclutador,  
**Quiero** que el sistema automatice las tareas repetitivas del proceso de contratación,  
**Para** reducir el tiempo administrativo y concentrarme en actividades de mayor valor.

**Criterios de Aceptación:**
1. El sistema debe generar comunicaciones personalizadas para candidatos en cada etapa del proceso.
2. Las entrevistas deben programarse automáticamente basándose en la disponibilidad de todos los participantes.
3. Los flujos de trabajo deben adaptarse dinámicamente según el tipo de posición y departamento.
4. El sistema debe enviar recordatorios a los evaluadores que no han completado sus tareas dentro del plazo establecido.
5. El proceso de onboarding debe iniciarse automáticamente cuando un candidato acepta una oferta.

**Categoría:** Automatización y Eficiencia

### 1.4 Historia de Usuario: Experiencia del Candidato

**Como** candidato,  
**Quiero** tener una experiencia de aplicación transparente y personalizada,  
**Para** sentirme valorado durante todo el proceso de contratación.

**Criterios de Aceptación:**
1. El proceso de aplicación debe ser intuitivo y adaptable a dispositivos móviles.
2. Debo recibir actualizaciones automáticas sobre el estado de mi aplicación en cada etapa.
3. La programación de entrevistas debe respetar mis preferencias de disponibilidad.
4. Debo recibir preparación personalizada para cada etapa del proceso de selección.
5. Si no soy seleccionado, debo recibir retroalimentación constructiva y la posibilidad de ser considerado para futuras oportunidades.

**Categoría:** Experiencia de Usuario

### 1.5 Historia de Usuario: Análisis Predictivo de Reclutamiento

**Como** director de recursos humanos,  
**Quiero** acceder a análisis predictivos sobre el proceso de reclutamiento,  
**Para** optimizar la estrategia de contratación y reducir costos.

**Criterios de Aceptación:**
1. El sistema debe predecir tiempos de contratación y tasas de conversión por canal de reclutamiento.
2. Debo poder identificar cuellos de botella en el proceso de contratación en tiempo real.
3. El sistema debe proporcionar análisis comparativo con benchmarks de la industria.
4. Debo poder generar informes personalizados para diferentes stakeholders.
5. El sistema debe ofrecer recomendaciones procesables para mejorar la eficiencia del proceso.

**Categoría:** Análisis y Reportes

## 2. Product Backlog

### 2.1 Priorización MoSCoW

#### Must Have (Debe tener)

1. **Emparejamiento Inteligente de Candidatos**
   - **Rationale:** Es la funcionalidad central diferenciadora del sistema y proporciona el valor principal a los reclutadores para identificar candidatos adecuados.
   - **Impacto:** Alto - Reduce significativamente el tiempo de selección y mejora la calidad de las contrataciones.

2. **Experiencia del Candidato**
   - **Rationale:** Una experiencia de candidato deficiente puede causar la pérdida de talentos valiosos.
   - **Impacto:** Alto - Mejora la tasa de conversión de candidatos y la percepción de marca empleadora.

#### Should Have (Debería tener)

3. **Colaboración en Tiempo Real**
   - **Rationale:** Mejora significativamente la eficiencia del proceso de evaluación pero depende del emparejamiento inteligente.
   - **Impacto:** Medio - Reduce los tiempos de toma de decisiones y mejora la calidad de evaluación.

4. **Automatización del Proceso de Contratación**
   - **Rationale:** Proporciona eficiencias operativas importantes pero no es tan diferenciador como las características de IA.
   - **Impacto:** Medio - Reduce tareas administrativas y errores humanos.

#### Could Have (Podría tener)

5. **Análisis Predictivo de Reclutamiento**
   - **Rationale:** Proporciona valor a largo plazo pero requiere datos acumulados de los procesos anteriores.
   - **Impacto:** Medio-Bajo inicialmente, aumentando con el tiempo - Mejora la toma de decisiones estratégicas.

#### Won't Have (No tendrá en esta fase)

- Integración completa con todos los sistemas HRIS del mercado
- Módulo avanzado de gestión del talento post-contratación
- Herramientas de evaluación psicométrica avanzada
- Portal de carrera completo para empleados internos

### 2.2 Proceso de Prompt Engineering

#### Prompt 1: Enfoque Basado en Funcionalidades

"Basado en el documento PRD del sistema LTI ATS, genera historias de usuario que cubran las funcionalidades principales del sistema. Para cada historia, incluye el rol, la acción deseada y el beneficio esperado. Añade al menos tres criterios de aceptación por historia."

**Análisis:** Este prompt inicial produjo historias de usuario básicas pero carecían de especificidad y no capturaban completamente la complejidad del sistema LTI ATS. Los criterios de aceptación eran demasiado genéricos.

#### Prompt 2: Enfoque Basado en Casos de Uso

"Revisa los casos de uso detallados en el PRD de LTI ATS (Reclutamiento Inteligente, Colaboración en Tiempo Real y Onboarding Automatizado) y transforma cada caso de uso en una o más historias de usuario siguiendo el formato estándar. Asegúrate de que cada historia sea independiente, negociable, valiosa, estimable, pequeña y testeable. Incluye al menos cinco criterios de aceptación específicos por historia."

**Análisis:** Este prompt generó historias de usuario mejor alineadas con los casos de uso del sistema, pero aún faltaba la conexión con las innovaciones diferenciadoras del sistema como el motor de IA y la experiencia humanizada.

#### Prompt 3: Enfoque Holístico con Énfasis en Valor Diferenciador

"Basado en el PRD completo de LTI ATS, especialmente en las secciones de Propuesta de Valor Única y Funcionalidades Principales, genera cinco historias de usuario cruciales que capturen la esencia innovadora del sistema. Cada historia debe seguir el formato 'Como [rol específico], quiero [funcionalidad claramente definida] para [beneficio concreto y medible]'. Incluye cinco criterios de aceptación detallados por historia que sean específicos, medibles y verificables. Asegúrate de que cada historia refleje uno de los pilares diferenciales: IA Contextual, Colaboración Omnicanal, Experiencia Humanizada, Automatización Adaptativa o Análisis Predictivo."

**Análisis:** Este prompt fue el más efectivo porque:
- Consideró el documento PRD completo pero enfatizó las secciones más relevantes
- Solicitó explícitamente historias que capturaran la esencia innovadora del sistema
- Requirió criterios de aceptación detallados y verificables
- Alineó cada historia con uno de los pilares diferenciales del sistema
- Resultó en historias más completas y representativas del valor único del sistema

**Elementos superiores del prompt ganador:**
1. **Especificidad contextual:** Referenció secciones específicas del PRD (Propuesta de Valor y Funcionalidades)
2. **Enfoque en diferenciadores:** Solicitó que cada historia reflejara un pilar diferencial del sistema
3. **Criterios de calidad claros:** Especificó que los criterios debían ser medibles y verificables
4. **Estructura bien definida:** Proporcionó el formato exacto esperado para cada historia
5. **Límite claro:** Especificó exactamente cinco historias, lo que forzó la priorización

## 3. Tickets Técnicos: Historia de Usuario 1

### 3.1 Implementación del Analizador Semántico de CV

**Título:** Implementar analizador semántico de CV con NLP avanzado

**Descripción Técnica:**
Desarrollar un componente de procesamiento de lenguaje natural capaz de extraer y comprender semánticamente información relevante de los CV de candidatos. El analizador debe identificar no solo palabras clave, sino comprender contexto, jerarquías de habilidades, responsabilidades, y logros. Debe utilizar transformers pre-entrenados para comprensión contextual del lenguaje y ser capaz de normalizar términos de la industria.

**Implementación:**
1. Utilizar la biblioteca Hugging Face Transformers con un modelo base BERT o RoBERTa fine-tuneado para el dominio de RRHH
2. Implementar procesadores específicos para secciones comunes de CV (educación, experiencia, habilidades)
3. Desarrollar un sistema de normalización para términos técnicos y roles de trabajo
4. Implementar un pipeline de preprocesamiento para diferentes formatos de CV (PDF, DOCX, HTML)
5. Crear una API RESTful que exponga esta funcionalidad al servicio de emparejamiento

**Definición de Done:**
- El analizador procesa correctamente al menos 95% de los formatos comunes de CV
- La extracción de entidades (habilidades, experiencia, educación) tiene una precisión mínima del 90%
- El sistema normaliza correctamente terminología técnica variada a conceptos estándar
- El tiempo de procesamiento no excede 2 segundos por CV
- Pruebas unitarias y de integración cubren al menos 85% del código
- Documentación completa de la API y arquitectura del componente

**Dependencias:**
- Acceso a conjuntos de datos de CV anonimizados para entrenamiento y pruebas
- Infraestructura de computación con GPU para entrenamiento de modelos
- Diccionario de normalización de términos técnicos y roles

**Consideraciones Técnicas:**
- Considerar implementación de procesamiento por lotes para optimizar rendimiento
- Implementar monitoreo de drift del modelo para detectar cambios en patrones de CV
- Garantizar que el procesamiento cumpla con normativas de privacidad como GDPR

### 3.2 Desarrollo del Motor de Vectorización de Perfiles

**Título:** Desarrollar motor de vectorización de perfiles de candidatos

**Descripción Técnica:**
Crear un sistema que transforme los perfiles de candidatos procesados por el analizador semántico en representaciones vectoriales multidimensionales (embeddings). Estas representaciones deben capturar la esencia de las habilidades, experiencia y atributos del candidato en un espacio vectorial que permita comparaciones semánticas sofisticadas.

**Implementación:**
1. Diseñar una arquitectura de embedding que combine diferentes aspectos del perfil (técnico, soft skills, experiencia)
2. Implementar algoritmos de Sentence-BERT para vectorizar descripciones textuales
3. Desarrollar técnicas de ponderación para diferentes componentes del perfil
4. Implementar técnicas de reducción de dimensionalidad para optimizar almacenamiento y búsqueda
5. Integrar con base de datos vectorial (Pinecone o Weaviate) para almacenamiento eficiente

**Definición de Done:**
- Los embeddings capturan efectivamente similitudes semánticas entre perfiles relacionados
- El sistema genera vectores consistentes para perfiles similares (verificado mediante pruebas de similaridad)
- La generación de vectores se completa en menos de 1 segundo por perfil
- Implementación de pruebas que validan la estabilidad de los embeddings
- Integración completa con la base de datos vectorial elegida
- Documentación de la arquitectura del componente y sus interfaces

**Dependencias:**
- Componente de análisis semántico de CV completado
- Infraestructura para base de datos vectorial configurada
- Acceso a conjuntos de datos para validación de similaridad

**Consideraciones Técnicas:**
- Evaluar regularmente la calidad de los embeddings mediante técnicas de validación intrínseca y extrínseca
- Implementar versionado de modelos para facilitar actualizaciones sin pérdida de consistencia
- Considerar técnicas de quantización para optimizar almacenamiento y rendimiento

### 3.3 Implementación del Algoritmo de Matching Semántico

**Título:** Implementar algoritmo de matching semántico candidato-vacante

**Descripción Técnica:**
Desarrollar el algoritmo central que realizará el emparejamiento entre candidatos y vacantes. Este componente debe utilizar las representaciones vectoriales para calcular similitudes multidimensionales, considerar factores como pesos dinámicos para diferentes criterios, y generar puntuaciones explicables de compatibilidad.

**Implementación:**
1. Diseñar un algoritmo de matching que utilice similaridad coseno entre vectores como base
2. Implementar sistema de pesos dinámicos que se ajusten según importancia relativa de criterios
3. Desarrollar componente de explicabilidad que identifique factores clave que contribuyen a cada match
4. Crear mecanismo de feedback para que el sistema aprenda de decisiones de contratación pasadas
5. Implementar optimizaciones para escalar a grandes volúmenes de candidatos

**Definición de Done:**
- El algoritmo identifica correctamente coincidencias relevantes en conjuntos de prueba (precision@10 > 0.8)
- Las explicaciones generadas son comprensibles y útiles para reclutadores (validado por usuarios de prueba)
- El sistema escala efectivamente hasta 100,000 candidatos con tiempo de respuesta < 3 segundos
- Mecanismo de feedback implementado y validado con datos históricos
- Pruebas automatizadas que validan resultados de casos de uso complejos
- Documentación completa de los parámetros del algoritmo y su lógica

**Dependencias:**
- Componente de vectorización de perfiles completado
- Componente de vectorización de vacantes completado (similar al de perfiles)
- Base de datos vectorial optimizada para búsquedas de similaridad

**Consideraciones Técnicas:**
- Implementar estrategias de caché para resultados frecuentes
- Considerar aproximaciones para búsquedas de similaridad a gran escala (HNSW, IVF)
- Diseñar para minimizar sesgos algorítmicos en el proceso de matching

### 3.4 Desarrollo de API para el Servicio de Emparejamiento

**Título:** Desarrollar API RESTful para el servicio de emparejamiento

**Descripción Técnica:**
Crear una API que exponga las capacidades del motor de emparejamiento cognitivo al resto del sistema. Esta API debe proporcionar endpoints para búsqueda de candidatos, generación de recomendaciones para vacantes, y retroalimentación sobre resultados de emparejamiento.

**Implementación:**
1. Diseñar una API RESTful con endpoints para los principales casos de uso
2. Implementar validación de parámetros y manejo de errores robusto
3. Desarrollar sistema de paginación y filtrado para grandes conjuntos de resultados
4. Implementar mecanismos de caché para optimizar consultas frecuentes
5. Crear documentación interactiva con Swagger/OpenAPI

**Definición de Done:**
- Todos los endpoints clave implementados y probados (búsqueda, recomendación, feedback)
- La API maneja correctamente errores y casos extremos
- Paginación y filtrado funcionan correctamente con grandes conjuntos de datos
- La latencia promedio de respuesta está dentro de los SLAs definidos (<500ms p95)
- Pruebas de carga demuestran que la API soporta al menos 100 solicitudes concurrentes
- Documentación completa de la API con ejemplos funcionales

**Dependencias:**
- Componente de algoritmo de matching semántico completado
- Infraestructura para despliegue de API configurada

**Consideraciones Técnicas:**
- Implementar rate limiting para prevenir abusos
- Considerar versioning de la API para futuras evoluciones
- Diseñar para observabilidad con logs estructurados y métricas relevantes

### 3.5 Creación de Interfaz de Presentación de Resultados

**Título:** Desarrollar interfaz de presentación de resultados de emparejamiento

**Descripción Técnica:**
Crear los componentes de frontend que mostrarán a los reclutadores los resultados de emparejamiento de manera intuitiva y accionable. La interfaz debe presentar puntuaciones multidimensionales, explicaciones sobre los matches, y facilitar acciones inmediatas.

**Implementación:**
1. Diseñar componentes React para visualización de listas de candidatos recomendados
2. Implementar visualizaciones para puntuaciones multidimensionales (gráficos radar, barras)
3. Desarrollar componentes para mostrar factores explicativos de cada recomendación
4. Crear controles para filtrado avanzado y organización de resultados
5. Implementar funcionalidades de acción inmediata (contactar, programar entrevista)

**Definición de Done:**
- Interfaz implementada según especificaciones de diseño
- Visualizaciones son intuitivas y comunican efectivamente la información (validado con usuarios)
- Los componentes son responsivos y se adaptan a diferentes tamaños de pantalla
- Las interacciones tienen tiempos de respuesta adecuados (<200ms)
- Pruebas de usabilidad completadas con al menos 5 usuarios potenciales
- Documentación de componentes y guía de estilo actualizada

**Dependencias:**
- API de emparejamiento completada y disponible
- Sistema de diseño y componentes base establecidos
- Mockups y especificaciones de diseño aprobados

**Consideraciones Técnicas:**
- Implementar renderizado optimizado para listas largas de resultados (virtualization)
- Considerar accesibilidad (WCAG 2.1) para todos los componentes
- Diseñar para internacionalización desde el inicio

## 4. Estimación de Esfuerzo

### 4.1 Metodología de Estimación

Para estimar el esfuerzo de implementación, utilizamos la secuencia de Fibonacci para story points (1, 2, 3, 5, 8, 13, 21), donde:

- 1 punto: Tarea muy simple, puede completarse en menos de medio día
- 2 puntos: Tarea simple, requiere aproximadamente un día
- 3 puntos: Tarea moderada, requiere 1-2 días
- 5 puntos: Tarea compleja, requiere 3-5 días
- 8 puntos: Tarea muy compleja, requiere 1-2 semanas
- 13 puntos: Tarea extremadamente compleja con incertidumbre, requiere 2-3 semanas
- 21 puntos: Tarea que probablemente necesita ser dividida, requiere más de 3 semanas

Los factores considerados para la estimación incluyen:
- Complejidad técnica
- Necesidad de investigación o prototipos
- Dependencias externas
- Experiencia previa del equipo
- Riesgo e incertidumbre
- Esfuerzo de pruebas y validación

### 4.2 Estimaciones por Historia de Usuario

#### HU1: Emparejamiento Inteligente de Candidatos - 21 SP

- Implementación del Analizador Semántico de CV: 8 SP
  - Justificación: Alta complejidad técnica, requiere investigación en NLP y modelos de ML específicos para el dominio.

- Desarrollo del Motor de Vectorización de Perfiles: 5 SP
  - Justificación: Complejidad media-alta, requiere conocimiento de embeddings y optimización.

- Implementación del Algoritmo de Matching Semántico: 5 SP
  - Justificación: Complejidad media-alta, con desafíos de rendimiento y optimización.

- Desarrollo de API para el Servicio de Emparejamiento: 3 SP
  - Justificación: Complejidad moderada, pero construida sobre componentes ya desarrollados.

- Creación de Interfaz de Presentación de Resultados: 3 SP
  - Justificación: Complejidad moderada, con enfoque en UX y visualización de datos.

#### HU2: Colaboración en Tiempo Real - 13 SP

- Implementación de sistema de colaboración en tiempo real: 8 SP
  - Justificación: Complejo por los requisitos de sincronización y manejo de concurrencia.

- Desarrollo de interfaz colaborativa para evaluaciones: 5 SP
  - Justificación: Complejidad media por los requisitos de UX y retroalimentación instantánea.

#### HU3: Automatización del Proceso de Contratación - 8 SP

- Desarrollo del motor de flujo de trabajo: 5 SP
  - Justificación: Complejidad media por la necesidad de adaptabilidad y reglas de negocio.

- Implementación de comunicaciones automatizadas: 3 SP
  - Justificación: Complejidad moderada, con plantillas dinámicas y personalización.

#### HU4: Experiencia del Candidato - 8 SP

- Portal de candidatos móvil-responsivo: 5 SP
  - Justificación: Complejidad media con énfasis en experiencia de usuario y adaptabilidad.

- Sistema de seguimiento y notificaciones: 3 SP
  - Justificación: Complejidad moderada, integración con múltiples canales.

#### HU5: Análisis Predictivo de Reclutamiento - 13 SP

- Motor de análisis predictivo: 8 SP
  - Justificación: Alta complejidad por algoritmos predictivos y manejo de grandes volúmenes de datos.

- Dashboards y visualizaciones avanzadas: 5 SP
  - Justificación: Complejidad media, con requisitos de visualización interactiva y personalización.

### 4.3 Tabla Resumen de Estimaciones

| Historia de Usuario | Story Points | Justificación |
|---------------------|--------------|---------------|
| HU1: Emparejamiento Inteligente | 21 | Núcleo de la propuesta de valor, alta complejidad técnica en IA/ML |
| HU2: Colaboración en Tiempo Real | 13 | Complejidad técnica en sincronización y manejo de concurrencia |
| HU3: Automatización del Proceso | 8 | Complejidad media en reglas de negocio y personalización |
| HU4: Experiencia del Candidato | 8 | Enfoque en UX y diseño responsivo con notificaciones multicanal |
| HU5: Análisis Predictivo | 13 | Alta complejidad en algoritmos predictivos y visualización avanzada |
| **TOTAL** | **63** | |

## 5. Apéndice: Suposiciones

Durante la elaboración de este documento, se han realizado las siguientes suposiciones:

1. **Infraestructura Técnica:** Se asume disponibilidad de infraestructura cloud para el procesamiento de IA y almacenamiento de datos, preferiblemente AWS o Google Cloud.

2. **Equipo de Desarrollo:** Se asume un equipo multidisciplinario con experiencia en desarrollo web moderno (React, Node.js), procesamiento de lenguaje natural, y bases de datos relacionales y NoSQL.

3. **Integración con Sistemas Externos:** Se asume que los sistemas externos (HRIS, calendarios, email) proporcionan APIs o webhooks para integración.

4. **Volumen de Datos:** Las estimaciones asumen un volumen inicial de hasta 100,000 candidatos y 1,000 vacantes activas.

5. **Cumplimiento Normativo:** Se asume que la implementación deberá cumplir con regulaciones de privacidad como GDPR, especialmente para el procesamiento de datos de candidatos.

6. **Disponibilidad de Datos de Entrenamiento:** Para los componentes de IA, se asume acceso a conjuntos de datos etiquetados o la capacidad de generarlos durante la implementación.

7. **Soporte para Múltiples Idiomas:** Se asume inicialmente soporte para español e inglés, con posibilidad de expansión a otros idiomas.

8. **Experiencia de Usuario:** Las historias de usuario asumen interfaces web y móviles modernas con altos estándares de usabilidad.
