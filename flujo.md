# Flujo de trabajo
El flujo de trabajo en el que trabajaremos desde que se asigna una tarea hasta la realización de esta.

## Índice
- [Tablero](#tablero)
- [Asignación de tareas](#asignar-tareas)
- [Ramas](#ramas)
- [Commits](#commits)
- [Subir cambios](#subir-cambios)

<h2 id='tablero'>Tablero</h2>
Antes de iniciar con el flujo de trabajo hay que conocer el tablero que enlista las tareas a realizar. En la tabla siguiente se enlistan los diferentes estados que tiene el tablero de trabajo.

| Estado               | Descripción |
|----------------------|-------------|
| To Do                | Issue que está lista para realizaarse en el Sprint |
| In Progress          | La tarea está siendo desarrollada |
| Code Review          | La tarea ya fue desarrollada pero necesita revisión |
| Code Review Approved | El código ya fue revisado pero no ha sido fusionado a la rama Development |
| Done                 | La tarea ya se encuentra en la rama Development |

<img width="1344" alt="image" src="https://github.com/desarrolladora-temp/.github/assets/5274471/5aade18d-61df-48de-98c7-6748b1e7da9e">

<h2 id='asignar-tareas'>Asignación de tareas</h2>
En cada Sprint se enlistaran las tareas que se tienen que realizar en dicho Sprint y cada persona tendrá una cantidad de tareas asignadas. Al momento de tener las tareas, todas tendrán el estado **To Do** 
y al momento de empezar a realizar una tarea se debe cambiar manualmente el estado a **In Progress** para tener un control de las tareas que se están trabajando en el momento de visualizar el tablero.

<h2 id='ramas'>Ramas</h2>
Las diferentes ramas que cuenta el repositorio son las siguientes:

| Nombre      | Descripción |
|-------------|-------------|
| main        | Es la rama que se utiliza en producción, también es la que contiene los cambios más estables |
| development | Es la rama con los últimos cambios, la cual es la que se estará tomando en cuenta al momento de desarrollar nuevas tareas|

Cuando se va a trabajar en una nueva tarea, se tiene que crear una nueva rama partiendo de la rama **development** la cual es exclusivamente para trabajar dicha tarea y debe tener ciertas convención al momento de nombrarlo.

El tipo de convención para nombrar las ramas es la siguiente: `<type>/<reference>/<name>`.

- `feature`: Ramas para nuevas funcionalidades.
- `bugfix`: Ramas para resolver bugs.
- `hotfix`: Ramas para resolver algo de alta prioridad.

Unos ejemplos de nombrar una rama dependiendo el nombre de una tarea serían:

- `feature/issue-3/create-login`
- `bugfix/issue-12/login-validations-not-working`
- `hotfix/no-ref/home-view-not-working`

**IMPORTANTE**: Los nombres de las ramas deben estar escritas en inglés.

<h2 id='commits'>Commits</h2>
Ya creada tu rama en la que vas a trabajar, también es importante nombrar convencionalmennte tus commits, algunas consideraciones a la hora de nombrarlos son:

- Los commits deben estar escritos en **inglés**
- Los commits deben estar escritos con verbos en presente
- Los commits deben estar hechos en modo imperativo
- Los commits deben seguir el siguiente formato: `<type>: <message>`

Tipos de commits:
- `feat`: New feature.
- `fix`: Bug fix.
- `docs`: Documentation.
- `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc).
- `refactor`: Changes that neither fix a bug nor add a feature.
- `perf`: Changes that improve performance.
- `test`: Adding missing tests.
- `chore`: Changes to the build process or auxiliary tools and libraries such as documentation generation.

Ejemplos:
- `git commit -m "feat: add password encryption"`
- `git commit -m "fix: fix login validation"`
- `git commit -m "docs: update README.md"`
- `git commit -m "style: fix indentation"`
- `git commit -m "refactor: rewrite button component"`
- `git commit -m "perf: improve performance"`
- `git commit -m "test: add test for login validation"`
- `git commit -m "chore: update react dependencies"`

<h2 id='subir-cambios'>Subir cambios</h2>
Teniendo la tarea ya hecha, es hora de subir la rama al repositorio de GitHub para poder hacer una Pull Request a la rama **developmment** y esperar a la revisión de código. Con esto tu ticket pasará del estado **In Progress** a **Code Review**.
Los escenarios son los siguientes: Te aceptan los cambios o te piden cambios a tu código.

En caso de que tus cambios sean aceptados, tu ticket pasará al estado **Code Review Approved** y deberás hacer merge para unificar tus cambios con la rama de desarrollo para que el resto de tus compañeros puedan bajar dichos cambios a sus repositorios locales finalizando tu ticket a **Done**.

En caso contrario y te pidan cambios a tu Pull Request, tu ticket pasará a **In Progress** nuevamente y simplemente sigue trabajando en la misma rama, crea el nuevo commit y subelo de nuevo, esto actualizará el Pull Request y volverá al paso de **Code Review**.
