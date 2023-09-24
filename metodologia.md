<h1 id='methodology'>Metodología de trabajo</h1>
La metodología para trabajar será la metodología ágil/agile utilizando el framework SCRUM.

## Índice
- [¿Qué es Agile?](#agile)
- [SCRUM Framework](#scrum)
- [Backlog Creation](#backlog-creation)
- [Sprint Planning](#sprint-planning)
- [Daily Scrum](#daily-scrum)
- [Backlog Grooming](#backlog-grooming)
- [Sprint Review](#sprint-review)
- [Stakeholder Demo](#demo)

<h2 id='agile'>¿Qué es Agile?</h2>
Agile es un enfoque de desarrollo de software y gestión de proyectos que se basa en valores y principios específicos destinados a fomentar la flexibilidad, la colaboración, la adaptabilidad y la entrega continua de valor a los clientes.
En pocas palabras, es una forma de trabajar que puede generar flexibilidad y mayor eficiencia al momento de desarrollar software.

La metodología agile se compone del siguiente manifesto:
- Individuals and interactions over processes and tools
- Working software over comprehensive documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan

<h2 id='scrum'>SCRUM Framework</h2>
El framework SCRUM es una receta para lograr desarrollo ágil preescribiendo una estricta serie de:

- Roles
- Eventos
- Artefactos

|Roles          | Descripción                                                          |
|-------------|------------------------------------------------------------------------|
|Product Owner| Es la persona que representa el interés del negocio dentro del equipo. |
|Scrum Master | Encargado de recordar cómo funciona SCRUM en el equipo                 |
|Developer    | El desarrollador del proyecto                                          |
|Stakeholder  | Clientes importantes que prueban la app para feedback                  |

|Eventos            | Descripción                                                            |
|-------------------|------------------------------------------------------------------------|
|Backlog creation   | Enlistar las funcionalidades que se tienen que realizar en el proyecto |
|Sprint planning    | Planificación de qué tareas se trabajarán en el sprint actual          |
|Daily scrum        | Meeting diaria para saber el estado actual de cada tarea               |
|Backlog grooming   | Redefinir el backlog a mitad del sprint (opcional)                     |
|Sprint review      | Preparación y recopilación del sprint para el demo                     |
|Stakeholder demo   | Meeting para mostrar los avances que se tienen al cliente              |
|Team retrospective | Discusión para saber qué fue bien, mal y mejoras a la hora de trabajar |

<h3 id='backlog-creation'>Backlog Creation</h3>
Para la creación del backlog se necesita la ayuda de **user stories**, los cuales se crean mediante la siguiente estructura:

> As a ____, I want to ____, so that ____ 

- El primer espacio en blanco se llena con el rol o tipo de usuario
- El segundo espacio se llena con la meta a lograr
- El tercero se llena con la razón de por qué se quiere lograr dicha meta

Los **user stories** deben seguir el acrónimo *INVEST*:
- **I**ndependent - No deben depender de otro
- **N**egotiable - Pueden ser cancelados o cambiados a cualquier momento
- **V**aluable - Deben ser significativos, dar valor al proyecto
- **E**stimable - Deben ser descriptivos y suficientemente pequeños para ser capaces de estimar facilmente
- **S**mall - Suficientemente pequeños para completarlo en un sprint
- **T**estable - Tener la claridad suficiente para diseñar tests

También deben tener las siguientes categorías en los cuerpos de cada *user story*:
- Acceptance Criteria - Representa el requerimiento mínimo para que el *user story* sea considerado hecho
- Estimation of Effort - Determinar cuánto trabajo llevará a cabo realizar dicho *user story*

<h3 id='sprint-planning'>Sprint Planning</h3>
En SCRUM, el trabajo se divide en incrementos llamados **sprints**. Los sprints tipicamente duran ciertas semanas.

- Al inicio de cada sprint, todo el equipo se junta para decidir qué tareas trabajar en dicho sprint
- El Product Owner presenta la lista de user stories en el Backlog
- Los desarrolladores rompen cada user story en tareas más pequeñas
- Cada tarea es asignada a un desarrollador

<h3 id='daily-scrum'>Daily Scrum</h3>
Cada día, el SCRUM Master y los desarrolladores se reúnen para discutir el estado de sus tareas. Cada desarrollador tiene tres preguntas:

- ¿Qué trabajaste la última vez?
- ¿Qué trabajarás ahora?
- ¿Hay algo que esté bloqueando tu progreso?

<h3 id='backlog-grooming'>Backlog Grooming</h3>
Cada Sprint, el Product Owner mantiene el Backlog, agregando nuevas User Stories, modificando antiguas, etc.

- A la mitad de cada Sprint, todo el equipo se junta para discutir estas agregaciones
- El equipo discute las nuevas User Stories, y el Product Owner las ordena apropiadamente en el Backlog
- No se agregará nunca nuevas User Stories al Sprint en curso, pero se pueden indexar en los siguientes Sprints

<h3 id='sprint-review'>Sprint Review</h3>
Al finalizar cada Sprint, el equipo se reúne para discutir acerca del trabajo realizado en todo el Sprint.

- Las User Stories no finalizadas se regresan al Backlog
- El equipo acuerda qué funcionalidades son buenas para mostrar al cliente

<h3 id='demo'>Stakeholder Demo</h3>
Todo el equipo se reúne con el cliente para hacer una demostración del trabajo realizado en el Sprint

- El Product Owner por lo general lidera la demo
- El cliente da feedback, sugiere agregaciones, cambios, etc
- El Product Owner agrega nuevas User Stories sugeridas por el cliente al Backlog
