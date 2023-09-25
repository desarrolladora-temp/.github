## Diagrama de Bases de Datos

### Tabla: Usuarios
| Campo       | Tipo de Datos | Descripción                  |
|-------------|---------------|------------------------------|
| id          | INT           | Identificador único del usuario |
| nombre      | VARCHAR(50)   | Nombre del usuario           |
| email       | VARCHAR(100)  | Dirección de correo electrónico |
| contraseña  | VARCHAR(100)  | Contraseña del usuario       |
| rol         | ENUM('Usuario Común', 'Anfitrión') | Rol del usuario |
| ubicación   | VARCHAR(100)  | Ubicación del usuario        |

### Tabla: SalonesDeEventos
| Campo       | Tipo de Datos | Descripción                  |
|-------------|---------------|------------------------------|
| id          | INT           | Identificador único del salón de eventos |
| nombre      | VARCHAR(100)  | Nombre del salón de eventos  |
| tipo        | VARCHAR(50)   | Tipo de salón de eventos     |
| precio      | DECIMAL(10, 2)| Precio por hora del salón    |
| horarios    | TEXT          | Horarios de disponibilidad   |
| anfitrión_id| INT           | ID del anfitrión que registra el salón |

### Tabla: Eventos
| Campo       | Tipo de Datos | Descripción                  |
|-------------|---------------|------------------------------|
| id          | INT           | Identificador único del evento |
| usuario_id  | INT           | ID del usuario que agenda el evento |
| salón_id    | INT           | ID del salón de eventos reservado |
| fecha       | DATE          | Fecha del evento             |
| hora        | TIME          | Hora del evento              |

### Tabla: AgendaAnfitrión
| Campo       | Tipo de Datos | Descripción                  |
|-------------|---------------|------------------------------|
| id          | INT           | Identificador único de la entrada de agenda |
| anfitrión_id| INT           | ID del anfitrión que gestiona la agenda |
| evento_id   | INT           | ID del evento reservado      |
| estado      | ENUM('Pendiente', 'Confirmado', 'Cancelado') | Estado de la reserva |

### Relaciones
- La tabla `Usuarios` tiene una relación uno a muchos con la tabla `Eventos` a través del campo `id` de usuario.
- La tabla `Usuarios` tiene una relación uno a muchos con la tabla `AgendaAnfitrión` a través del campo `id` de usuario.
- La tabla `SalonesDeEventos` tiene una relación uno a muchos con la tabla `Eventos` a través del campo `id` de salón.
- La tabla `SalonesDeEventos` tiene una relación uno a muchos con la tabla `AgendaAnfitrión` a través del campo `id` de salón.
- La tabla `Usuarios` tiene una relación uno a muchos con la tabla `SalonesDeEventos` a través del campo `id` de anfitrión en caso de que el usuario sea un anfitrión.

