# Contexto Usuario Anónimo

## Características
Podrá realizar consultas al catálogo de productos y navegar de forma libre por la zona pública de la web.
## Escenarios como Usuario Anónimo

### Escenario registrar usuario
##### El usuario anónimo para registrarse con éxito deberá introducir: correo electrónico, contraseña, nombre, apellidos, dirección y teléfono. 
##### Los requisitos del sistema para hacer un registro correcto son: todos los campos del formulario tienen que estar rellenos, la contraseña tiene que tener más de 6 caracteres, el correo electrónico debe tener un formato (nombre)@(algo).(cualquier extensión)

+ **Como** Usuario anónimo
+ **Quiero** Registrar
+ **Para** Poder acceder a la web bajo un perfil para poder acceder a los privilegios de usuario

#### Criterios de aceptación
 **Escenario 1:** Usuario anónimo deja un campo vacío

- **Dado que** Usuario ha dejado uno o mas campos del formulario sin información
- **Cuando** Usuario ha pulsado el botón registrar
- **Entonces** Se muestra mensaje de informando que no puede dejar ningún campo de texto de información 

 **Escenario 2:** Usuario anónimo no introduce un formato correcto de contraseña

- **Dado que** Usuario ha introducido una contraseña de un formato que no corresponde con los requisitos del sistema que son mínimo 6 caracteres 
- **Cuando** Usuario ha ha pulsado el botón registrar
- **Entonces** Se muestra mensaje de error informando que la contraseña nueva no puede ser inferior a 6 caracteres

**Escenario 3:** Usuario anónimo introduce los datos correctamente

- **Dado que** Usuario ha rellenado todos los campos de texto
- **Cuando** Usuario ha pulsado el botón registrar
- **Entonces** Se muestra mensaje de informando que el usuario ha sido cambiado con éxito y se guardan en la base de datos

#### Descripción Funcional del Proceso Registrar usuario

1. El usuario selecciona la opción de darse de alta en el sistema
2. El sistema le muestra al usuario un formulario con los datos que debe rellenar para poder acceder al sistema
3. El usuario rellena los datos del formulario y pulsa botón registrar
4. El sistema comprueba que todos los datos son correctos
5. El sistema indica al usuario que el proceso de alta ha sido correcto y ya puede acceder a la web con sus datos

