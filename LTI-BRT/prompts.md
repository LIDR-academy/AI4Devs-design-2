
MODELO: ChatGPT4o

----

PROMPT #1


Actúa como un product Manager

# Tarea
Desarrolla 5 historias de usuario siguiendo la documentación aportada.

## Contexto
- Estamos desarrollando **las tareas** para llevar a cabo un proyecto **ATS**
- La empresa para la que estamos trabajando se llama **LTI**
- Se te ha facilitado la documentación de un PRD inicial con algunas de las funcionalidades claves que tendrá el sistema

## Respuesta
- Debes retornar la respuesta de cada historia de usuario en formato markdown ```markdown
- Utiliza un formato detallado de cada uno de los casos de uso.
- El formato de cada historia de usuario debe seguir la siguiente plantilla: 
```markdown
# Historia de usuario
Como [Rol] quiero [acción que debe poder realizar el usuario] para [beneficio que se espera del usuario]

>Ejemplo:
>
> Como gerente de producto, quiero una manera en que los miembros del equipo puedan entender cómo las tareas individuales contribuyen a los objetivos, para que puedan priorizar mejor su trabajo.

# Criterios de aceptación
[Crea 5 criterios de aceptación]

## Notas adicionales 
[agrega notas adicionales si consideras necesario aclarar conceptos de la historia]

## Historias de usuario relacionadas
[Agrega las historias de usuario relacionadas si lo consideras necesario]

```


----

PROMPT #2

Actúa ahora como Product Analyst

# Tarea
Prioriza cada historia de usuario para generar un backlog coherente de historias de usuario.

## Contexto
- La empresa cuenta con el siguiente stack tecnológico: React, Mysql, RabbitMQ, PostgreSQL, PHP, Symfony Framework, Nodejs, Typescript y Nextjs

## Consideraciones
- Debes priorizar en este sentido: Impacto en el producto -> Esfuerzo o StoryPoints necesarios -> Tecnología necesaria
- Deberás tener en cuenta el stack de la empresa
- No es necesario que elijas todo el stack solo los que realmente sea necesario para desarrollar las funcionalidades del proyecto.
- Indica en cada una de ellas el motivo por el cual se ha priorizado 

## Salida
- Debes devolver el resultado indicando por orden las historias de usuario en base a su prioridad.
- Devuelve la salida de cada prioridad en formato markdown ```markdown.



----

PROMPT #3

# Tarea
Como experto en planificación de proyectos genera los tickets de la historia de usuario de la historia de usuario con prioridad 1.

## Contexto
- El equipo de trabajo está compuesto por 2 desarrolladores Juniors, 1 Senior y 1 Tech Lead.

## Consideraciones
- Sigue la estimación con la metodología story points para poder evaluar a posteriori el progreso y los sprints siguientes
- Los sprints son de 10 días laborables.
- Las categorias que usaremos en cada ticket son: **Feature**, **Tarea Tecnica**, **Bugs/Errores**, **Mejoras**, **Investigacion**.
- Prioriza también a través del impacto de cada ticket en el sistema: **Critico**, **Alto**, **Medio** y **Bajo**

## Salida
- Cada ticket de trabajo debe tener el siguiente formato:
```markdown
    # Ticket #[Número de ticket ]: [Título]
    
    ## Descripción
    [Descripción detallada del ticket]

    ## Criterios de aceptación
    [Al menos 3 criterios de aceptación]

    ## Prioridad
    [Prioridad indicada en el ticket]

    ## Estimación de esfuerzo
    [Estimación según la metodología mencionada]

    ## Asignado
    [Persona asignada al ticket]

    ## Categoría
    [Categoría del ticket]

    ## Comentarios
    [Comentarios adicionales para aclarar conceptos sobre el ticket]

```
- Denes retornar cada ticket en formato markdown con ```markdown