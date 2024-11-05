# Chatbot: ChatGPT-4.0

# Prompts

## Prompt 1

Te voy a pasar un archivo en formato markdown con la definición inicial de un proyecto, haz el análisis y con pase en eso, crea un PRD con el formato estándar para complementar la documentación, no me contestes nada por ahora, el PRD tiene que ser en formato markdown 

Adjunte el archivo LTI-LAGV.md

## Respuesta chatGPT

Gracias por subir el archivo. Voy a revisarlo y prepararé el PRD en formato Markdown para complementar la documentación.

He revisado el contenido inicial del archivo. Con base en el análisis del documento que define el Applicant-Tracking System (ATS) de LTI, voy a estructurar un Documento de Requisitos del Producto (PRD) para complementar la documentación existente. Este PRD incluirá:

1. **Resumen Ejecutivo**
2. **Objetivos del Proyecto**
3. **Alcance del Producto**
4. **Requisitos Funcionales**
5. **Requisitos No Funcionales**
6. **Casos de Uso**
7. **Especificaciones de Diseño**
8. **Criterios de Aceptación**
9. **Consideraciones Técnicas**

Voy a proceder a crear el PRD en formato Markdown, ajustándolo a los detalles proporcionados en el archivo original.


## Prompt 2

Ya que tienes todo el contexto del proyecto, en este ejercicio vas a actuar como un Product Manager y Business Analyst, tu misión es generar la siguiente documentación para empezar a implementar el ATS:

1) Generar las **User Stories**, para este paso debes implememtar todas las que sean posibles siguiendo el siguiente formato:

    **Título de la Historia de Usuario:** 
    1. Como [rol del usuario],
    2. quiero [acción que desea realizar el usuario],
    3. para que [beneficio que espera obtener el usuario].

    **Criterios de Aceptación:**
    1. [Detalle específico de funcionalidad]
    2. [Detalle específico de funcionalidad]
    3. [Detalle específico de funcionalidad]

    **Notas Adicionales:**
    * [Cualquier consideración adicional]

    **Historias de Usuario Relacionadas:**
    * [Relaciones con otras historias de usuario]


2) Arma el **Backlog de producto** con las User Stories, priorizándolas como consideres conveniente acorde a alguna metodología concreta.

3) Elige la User Story más importantes y genera los Tickets de trabajo. Aterrízalos técnicamente, tal y como se hace en las reuniones de planificación.

4) Estima el esfuerzo de los tickets de trabajo usando la metodología (fibonacci, poker, tallas de camiseta) y unidades (horas, puntos de historia).


Todos esos puntos se deben atender basándole completamente de la documentación que te pasé y del PRD que genereaste previamiente.

Hazme las preguntas que necesites antes de iniciar y no generes nada por el momento, vamos a ir punto por punto y así sucesivamente hasta cubrir loscuatro entregables.


## Respuesta ChatGPT

Para comenzar, tengo algunos puntos de confirmación que me ayudarán a definir las entregas de manera precisa:

1. **Roles de usuario**: ¿Debo asumir únicamente a reclutadores, managers y candidatos como los roles principales, o hay algún otro que deba considerar en las historias de usuario? 
   
2. **Metodología para el backlog**: Para la priorización del backlog, ¿prefieres una metodología en particular, como MoSCoW o RICE, o dejas la elección a mi criterio?

3. **Estándar de estimación**: ¿Hay alguna metodología específica para estimar el esfuerzo de los tickets que prefieras, como puntos de historia o alguna combinación de tallas de camiseta con horas?

Con estas respuestas puedo estructurar mejor cada entrega.


## Prompt 3
1) Por el momento esos son todos los roles que debes considerar
2) Cuál metodología me conviene ocupar y por qué
3) Cuales metodologías me conviene convinas y por qué



## Respuesta ChatGPT 

Excelente, aquí te doy algunas recomendaciones para las metodologías:

### 2) **Metodología para el backlog**  
Te sugiero utilizar **MoSCoW** (Must have, Should have, Could have, y Won’t have) para la priorización de las historias de usuario en el backlog. Aquí te explico por qué:

- **Simplicidad y claridad**: MoSCoW permite dividir las historias en categorías claras según su importancia, ayudando a centrar el desarrollo en lo esencial (lo que “Must have”) sin descuidar las funciones adicionales que aportan valor (como “Should have” y “Could have”).
- **Adaptabilidad en sprints**: Puedes re-evaluar prioridades de manera flexible al término de cada sprint. Esto es ideal en proyectos como un ATS, que pueden tener ajustes rápidos según las pruebas o las necesidades de los usuarios.
- **Enfoque en el MVP**: Esta metodología es útil para definir el mínimo producto viable (MVP) al establecer claramente qué es fundamental para el primer lanzamiento. Esto es crucial en productos como el ATS, donde funcionalidades clave (como la clasificación de CVs) deben ser entregadas antes que otras menos críticas (por ejemplo, el análisis de tono).

### 3) **Métodos de estimación para tickets de trabajo**

Para la estimación del esfuerzo, recomendaría una **combinación de puntos de historia** con una **escala de Fibonacci** (1, 2, 3, 5, 8, etc.):

- **Puntos de historia** permiten estimar el esfuerzo relativo considerando tanto la complejidad como el tiempo. Esta metodología ayuda a visualizar mejor el avance del proyecto en términos de esfuerzo, lo que resulta valioso para productos complejos como el ATS.
- **Escala de Fibonacci**: Esta escala no lineal refleja mejor el esfuerzo requerido, especialmente en tareas que tienden a volverse más complejas conforme aumenta su tamaño.

Para complementar esta estimación, podemos asignar valores de **tallas de camiseta** (XS, S, M, L, XL) en base a los puntos de historia. Esto permite categorizar de forma rápida el esfuerzo de cada ticket y facilita la planificación de los sprints, ya que los equipos pueden visualizar mejor la carga de trabajo de forma más general.

¿Te parece bien esta combinación de metodologías para avanzar con las entregas?


## Prompt 4

SÍ, me parece bien, vamos a comenzar con el punto 1 que es Generar las **User Stories**, no olvides seguir el formato que te compartí.

## Respuesta ChatGPT 
Perfecto, aquí te comparto las primeras **User Stories** basadas en el análisis del ATS. Estas están enfocadas en cubrir las funcionalidades clave descritas en el PRD, tales como la clasificación de CVs, la evaluación automatizada, el chat en vivo y la automatización de recordatorios.

¿Te gustaría continuar con más historias de usuario en función de los detalles del PRD, o deseas ajustar alguna de estas antes de proseguir?

## Prompt 5
Vamos a hacer unas modificaciones antes de crear más historias de usuarios. 
Con el fin de darle una mejor estructura, vamos a enumerar cada historia de usuario, por ejemplo, la primera sería:

1. Clasificación Automática de CVs

La segunda sería:
2. Evaluación Automatizada de Candidatos

Es decir, cada título tiene que tener su respectivo número de historia de usuario

## Respuesta ChatGPT 
Me dio las historias de usuario

¿Te gustaría que continuemos con nuevas historias de usuario o deseas alguna otra modificación en las ya existentes?

## Prompt 6

Continua generando más historias de usuario

## Respuesta ChatGPT 

Se generaron otras 5 historias de usuario para un total de 10.

¿Te gustaría que continúe generando más historias o necesitas algún ajuste en estas?

## Prompt 7

No, con estás 10 historias de usuario es suficiente, guárdalas para que posteriormente me hagas un archivo en formato markdown con esta información para cubrir el primer punto.

Vamos a seguir con el segundo punto: Arma el **Backlog de producto** con las User Stories.

## Respuesta ChatGPT 

A continuación, he organizado el Backlog de producto para priorizar las historias de usuario, aplicando la metodología MoSCoW para la clasificación:

 ¿Te gustaría que iniciemos con el desglose de la historia más prioritaria en tickets de trabajo?

## Prompt 8

Vamos a complementar este punto con una tabla en markdown con esta misma información y también considerando lo siguiente:

- Impacto en el usuario y valor del negocio.
- Urgencia basada en tendencias del mercado y feedback de usuarios.
- Complejidad y esfuerzo estimado de implementación.
- Riesgos y dependencias entre tareas.

## Respuesta ChatGPT 

Para complementar tu documento de proyecto con las tablas solicitadas en formato Markdown, aquí tienes un ejemplo. Las tablas reflejan la misma información que las historias de usuario y añaden los nuevos criterios que mencionaste.

## Prompt 9

De la primera tabla, tabla 1: Historias de Usuario, no entiendo la cómo se relaciona la prioridad (alta, baja, media) con la metodología MUSCoW, agrega las columnas que hagan falta o haz lo cambios que se necesiten

## Respuesta ChatGPT 

Claro, aquí tienes la tabla de Historias de Usuario modificada para incluir solo dos columnas: Historia de Usuario y Prioridad (MoSCoW). He incluido los números y nombres de las historias:

## Prompt 10

De la tabla de Historias de Usuario, vamos a hacer las siguintes modificaciones:
La tabla únicamente va tener dos columnas, Historia de Usuario y Prioridad (MoSCoW), la columna de historia de usuario debe tener el número y nombre de la historia de usuario, la columna Prioridad, se queda igual.

## Respuesta ChatGPT 

Generó la tabla correctamente.

## Prompt 11

Listo, guarda las últimas versiones de las tablas (Tabla 1: Historias de Usuario, Tabla 2: Evaluación del Backlog), esto lo vamos a meter en el punto 2.

Genera el punto 3: Elige la User Story más importantes y genera los Tickets de trabajo.

Básate en la siguiente  estructura:

1. Título Claro y Conciso
Un resumen breve que refleje la esencia de la tarea. Debe ser lo suficientemente descriptivo para que cualquier miembro del equipo entienda rápidamente de qué se trata el ticket.


2. Descripción Detallada
Propósito: Explicación de por qué es necesaria la tarea y qué problema resuelve.
Detalles Específicos: Información adicional sobre requerimientos específicos, restricciones, o condiciones necesarias para la realización de la tarea.

3. Criterios de Aceptación
Expectativas Claras: Lista detallada de condiciones que deben cumplirse para que el trabajo en el ticket se considere completado.
Pruebas de Validación: Pasos o pruebas específicas que se deben realizar para verificar que la tarea se ha completado correctamente.

4. Prioridad
Nivel de Urgencia: Una clasificación de la importancia y la urgencia de la tarea, lo cual ayuda a determinar el orden en que deben ser abordadas las tareas dentro del backlog.

5. Estimación de Esfuerzo
Puntos de Historia o Tiempo Estimado: Una evaluación del tiempo o esfuerzo que se espera que tome completar el ticket. Esto es esencial para la planificación y gestión del tiempo del equipo.

6. Asignación
Responsable: Quién o qué equipo será responsable de completar la tarea. Esto asegura que todos los involucrados entiendan quién está a cargo de cada parte del proyecto.

7. Etiquetas o Tags
Categorización: Etiquetas que ayudan a clasificar el ticket por tipo (bug, mejora, tarea, etc.), por características del producto (UI, backend, etc.), o por sprint/versión.

8. Comentarios y Notas
Colaboración: Espacio para que los miembros del equipo agreguen información relevante, hagan preguntas, o proporcionen actualizaciones sobre el progreso de la tarea.

9. Enlaces o Referencias
Documentación Relacionada: Enlaces a documentos, diseños, especificaciones o tickets relacionados que proporcionen contexto adicional o información necesaria para la ejecución de la tarea.

10. Historial de Cambios
Rastreo de Modificaciones: Un registro de todos los cambios realizados en el ticket, incluyendo actualizaciones de estado, reasignaciones y modificaciones en los detalles o prioridades.

Y también toma como base este ejemplo:

**Título**: Implementación de Autenticación de Dos Factores (2FA)

**Descripción**: Añadir autenticación de dos factores para mejorar la seguridad del login de usuarios. Debe soportar aplicaciones de autenticación como Authenticator y mensajes SMS.

**Criterios de Aceptación:**
Los usuarios pueden seleccionar 2FA desde su perfil.
Soporte para Google Authenticator y SMS.
Los usuarios deben confirmar el dispositivo 2FA durante la configuración.
Prioridad: Alta

**Estimación**: 8 puntos de historia

**Asignado a**: Equipo de Backend

**Etiquetas**: Seguridad, Backend, Sprint 10

**Comentarios**: Verificar la compatibilidad con la base de usuarios internacionales para el envío de SMS.

**Enlaces**: Documento de Especificación de Requerimientos de Seguridad

**Historial de Cambios**:
01/10/2023: Creado por [nombre]
05/10/2023: Prioridad actualizada a Alta por [nombre]

## Respuesta ChatGPT 

Estos tickets están listos para ser incluidos en la planificación del equipo. Si necesitas más información o ajustes adicionales, házmelo saber.

## Prompt 12

Listo, guarda esta información para posteriormente agregarla en el punto 3: Elige la User Story más importantes y genera los Tickets de trabajo.

Por último, genera el punto 4:  Estima el esfuerzo de los tickets de trabajo. 

Ocupa todos lo datos que has recopilado hasta el momento, incluyendo los **Métodos de estimación para tickets de trabajo** que propusiste previamente.

## Respuesta ChatGPT 

Aquí tienes el punto 4 que incluye la estimación del esfuerzo de los tickets de trabajo utilizando la metodología que propones:

## Prompt 13

Te faltó el indice y la información del punto 3 y 4 ya no es la misma que anteriormente me había dado.

## Respuesta ChatGPT 

Mis disculpas por la confusión. A continuación, te presento la documentación completa, incluyendo el índice y actualizando los puntos 3 y 4 según la información anterior:

## Prompt 14

Te voy a pasar el archivo markdown final,  déjalo como está pero agrega una tabla en la parte inferior del  apartado 3 (Tickets de Trabajo), con el resumen, de los ticket de trabajo, y con ese mismo título "Resumen de tickets de trabajo", la tabla debe tener tres columnas:
1) ID
2) Ticket
3) Historia de Usuario Relacionada

## Respuesta ChatGPT 

Aquí tienes el archivo markdown con la tabla añadida en la sección "Tickets de Trabajo"

## Prompt 15

Pásame la table con las 3 columnas que especifiqué:
1) ID
2) Ticket
3) Historia de Usuario Relacionada

## Respuesta ChatGPT 

Aquí tienes la tabla actualizada 

## Prompt 16

Agrega la columna ID y haz la relación con la tabla de Resumen de Tickets de Trabajo

## Respuesta ChatGPT 

Aquí tienes la tabla actualizada 

## Prompt 17

Agrega los 10 casos de uso en las tablas del punto 3 y 4

## Respuesta ChatGPT 

Aquí tienes las tablas actualizadas, incluyendo las 10 historias de usuario.


# Conclusión - Generación de backlog

Le pasé como contexto toda la documentación de la sesión anterior y también desde un inicio pedí generar un archivo PRD, una vez con el contexto, considero que la pregunta clave del prompt fue:

"Hazme las preguntas que necesites antes de iniciar y no generes nada por el momento, vamos a ir punto por punto y así sucesivamente hasta cubrir loscuatro entregables."

Con eso, el chatbot me guió para elegir una metodología para crear el backlog (Ver prompt del 1 al 4).

Con eso y la explicación que me dio, fue bastante sencillo crear el backlog, simplemente lo complementé con otra tabla como la que se mostraba en los materiales previos a hacer el ejercicio. 

