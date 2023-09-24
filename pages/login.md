# Iniciar sesión
Este documento es para definir los requerimientos funcionales y no funcionales de la pantalla de inicio de sesión. Para ver cómo se ve la UI, entra al diseño en [Figma](https://www.figma.com/file/uHHtLosPfj8Ubvvz560Bkg/Mitote-(Copy)?type=design&node-id=101%3A13&mode=design&t=g55U5HP8l8Ggbw6n-1)

| **ID** | **Descripción** | **Detalle** |
|--------|-----------------|-------------|
| RF01   | Formulario de Inicio de Sesión | La pantalla debe incluir un formulario con campos para correo electrónico y contraseña, así como un botón *Iniciar Sesión*. |
| RF02   | Validación de Entrada | - El correo electrónico debe estar en formato válido.<br> - La contraseña debe tener al menos 8 caracteres y ser sensible a mayúsculas y minúsculas. |
| RF03   | Recuperación de Contraseña | Se debe proporcionar un enlace o botón para permitir a los usuarios restablecer su contraseña dando click en el texto *¿Olvidaste tu contraseña?*. |
| RF04   | Mensajes de Error | - Mostrar mensaje de error si no se ha llenado los campos <br> - Mostrar mensaje de error en caso de que el usuario o contraseña no coincida. |
| RF05   | Inicio de Sesión Exitoso | Después de un inicio de sesión exitoso, redirigir al usuario a la página principal y almacenar una cookie o sesión de inicio de sesión. |

## Casos de Uso
A continuación, se describen algunos casos de uso típicos para la pantalla de inicio de sesión:

- Un usuario registrado inicia sesión con éxito proporcionando un correo electrónico y contraseña válidos.
- Un usuario registrado intenta iniciar sesión con datos incorrectos y recibe un mensaje de error.
- Un usuario olvida su contraseña y utiliza la opción de recuperación de contraseña.
