# Contexto Administrador

## Características
Administrador será el encargado de realizar todas las funciones de gestión del sistema, modificaciones de usuarios y productos, mantenimiento de la base de datos y comprobación del buen funcionamiento de la Web
## Escenarios como Administrador

### Escenario añadir usuario
+ **Como** Administrador
+ **Quiero** Añadir Usuario
+ **Para** Tener un usuario registrado en el sistema

#### Criterios de aceptación
 **Escenario 1:** Administrador esta en pantalla de administrador y añade un nuevo usuario

- **Dado que** que el Administrador esta en pantalla de administrador y quiere añadir un nuevo usuario
- **Cuando** Administrador ha pulsado botón añadir usuario
- **Entonces** Se muestra pagina de formulario igual a la que se mostrará para los usuarios anónimos que se quieran registrar

**Escenario 2:** Administrador deja un campo vacío

- **Dado que** Administrador ha dejado uno o mas campos del formulario sin información
- **Cuando** Administrador ha pulsado el botón registrar
- **Entonces** Se muestra mensaje de informando que no puede dejar ningún campo de texto sin información

**Escenario 3:** Administrador cambia los datos correctamente

- **Dado que** Administrador ha rellenado todos los campos de texto
- **Cuando**  Administrador ha pulsado el botón registrar
- **Entonces** Se muestra mensaje de informando que los datos han sido cambiados con éxito y se guardan en la base de datos

**Escenario 4:** Administrador no introduce un formato correcto de contraseña

- **Dado que** Administrador ha introducido una contraseña de un formato que no corresponde con los requisitos del sistema que son mínimo 6 caracteres 
- **Cuando** Administrador ha pulsado el botón registrar
- **Entonces** Se muestra mensaje de error informando que la contraseña nueva no puede ser inferior a 6 caracteres

 


### Escenario modificar usuario
+ **Como** Administrador
+ **Quiero** modificar usuario
+ **Para** Tener acceso a modificar los datos de un usuario

#### Criterios de aceptación
 **Escenario 1:** Administrador deja un campo vacío

- **Dado que** Administrador ha dejado uno o mas campos del formulario sin información
- **Cuando** Administrador ha pulsado el botón modificar datos
- **Entonces** Se muestra mensaje de informando que no puede dejar ningún campo de texto de información

**Escenario 2:** Administrador cambia los datos correctamente

- **Dado que** Administrador ha rellenado todos los campos de texto
- **Cuando** Administrador ha pulsado el botón modificar datos
- **Entonces** Se muestra mensaje de informando que los datos han sido cambiados con éxito y se guardan en la base de datos

### Escenario eliminar usuario
+ **Como** Administrador
+ **Quiero** eliminar usuario
+ **Para** Poder eliminar los datos de un usuario del sistema

**Escenario 1:** Administrador elimina un usuario 

- **Dado que** Administrador está en la pantalla de un usuario 
- **Cuando** Administrador ha pulsado el botón eliminar usuario
- **Entonces** Se muestra mensaje de que el usuario fue eliminado y se elimina de la base de datos 

### Escenario añadir producto
+ **Como** Administrador
+ **Quiero** añadir producto
+ **Para** Poder añadir un producto al sistema

### Escenario modificar producto
+ **Como** Administrador
+ **Quiero** modificar producto
+ **Para** Poder modificar el nombre la descripción o el precio de un producto

### Escenario eliminar producto
+ **Como** Administrador
+ **Quiero** eliminar producto
+ **Para** Poder eliminar un producto del sistema