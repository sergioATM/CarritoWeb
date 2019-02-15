# Contexto Administrador

## Características
Administrador será el encargado de realizar todas las funciones de gestión del sistema, modificaciones de usuarios y productos, mantenimiento de la base de datos y comprobación del buen funcionamiento de la Web
## Escenarios como Administrador

### Escenario añadir usuario
+ **Como** Administrador
+ **Quiero** Añadir Usuario
+ **Para** Tener un usuario registrado en el sistema

#### Criterios de aceptación
 **Escenario 1:** Administrador esta en pantalla de administración, quiere añadir un usuario y rellena los datos correctamente

- **Dado que** que el Administrador esta en pantalla de administración y quiere añadir un nuevo usuario y ha rellenado todos los campos de texto
- **Cuando** Administrador ha pulsado botón añadir usuario
- **Entonces** Se muestra mensaje de informando que los datos han sido cambiados con éxito, se guardan en la base de datos y se publica el producto

**Escenario 2:** Administrador deja un campo vacío al querer añadir un usuario

- **Dado que** Administrador ha dejado uno o mas campos del formulario sin información
- **Cuando** Administrador ha pulsado el botón añadir usuario
- **Entonces** Se muestra mensaje informando que no puede dejar ningún campo de texto sin información


**Escenario 3:** Administrador no introduce un formato correcto de contraseña

- **Dado que** Administrador ha introducido una contraseña de un formato que no corresponde con los requisitos del sistema
- **Cuando** Administrador ha pulsado el botón añadir usuario
- **Entonces** Se muestra mensaje de error informando que el formato de la contraseña no cumple con los requisitos del sistema que son mas de 6 caracteres 
 


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
+ 
#### Criterios de aceptación
**Escenario 1:** Administrador elimina un usuario 

- **Dado que** Administrador está en la pantalla de administración
- **Cuando** Administrador ha pulsado el botón eliminar usuario
- **Entonces** Se muestra mensaje de que el usuario fue eliminado y se elimina de la base de datos 

### Escenario añadir producto
+ **Como** Administrador
+ **Quiero** añadir producto
+ **Para** Poder añadir un producto al sistema

#### Criterios de aceptación
 **Escenario 1:** Administrador esta en pantalla de administrador y añade un nuevo producto. Para añadir el nuevo producto tendrá que cumplir los siguientes requisitos: rellenar los campos de texto Nombre, Precio y Descripción y también tendrá que añadir una foto del producto.

- **Dado que** que el Administrador esta en pantalla de administración y ha cumplido todos los requisitos para añadir un producto.
- **Cuando** Administrador ha pulsado botón añadir producto
- **Entonces** Se muestra mensaje de que el producto se ha añadido correctamente

**Escenario 2:** Administrador esta en pantalla de administración y deja un campo vacío o no sube una imagen

- **Dado que** Administrador ha dejado uno o mas campos del formulario sin información o no ha subido foto del producto
- **Cuando** Administrador ha pulsado el botón añadir producto
- **Entonces** Se muestra mensaje de informando que no puede dejar ningún campo de texto sin información y que es obligatorio subir una foto.

**Escenario 3:** Administrador no introduce un formato correcto de imagen

- **Dado que** Administrador ha introducido una imagen de un formato que no corresponde con los requisitos del sistema
- **Cuando** Administrador ha pulsado el botón añadir producto
- **Entonces** Se muestra mensaje de error informando que el formato de la imagen no es el correcto y se muestran las opciones de los formatos admitidos.

### Escenario modificar producto
+ **Como** Administrador
+ **Quiero** modificar producto
+ **Para** Poder modificar el nombre la descripción o el precio de un producto

#### Criterios de aceptación
 **Escenario 1:** Administrador deja un campo vacío

- **Dado que** Administrador ha dejado uno o mas campos del formulario sin información
- **Cuando** Administrador ha pulsado el botón modificar datos
- **Entonces** Se muestra mensaje de informando que no puede dejar ningún campo de texto de información

**Escenario 2:** Administrador cambia los datos correctamente

- **Dado que** Administrador ha rellenado todos los campos de texto
- **Cuando** Administrador ha pulsado el botón modificar datos
- **Entonces** Se muestra mensaje de informando que los datos han sido cambiados con éxito y se guardan en la base de datos

**Escenario 3:** Administrador no introduce un formato correcto de imagen

- **Dado que** Administrador ha introducido una imagen de un formato que no corresponde con los requisitos del sistema
- **Cuando** Administrador ha pulsado el botón añadir producto
- **Entonces** Se muestra mensaje de error informando que el formato de la imagen no es el correcto y se muestran las opciones de los formatos admitidos.

### Escenario eliminar producto
+ **Como** Administrador
+ **Quiero** eliminar producto
+ **Para** Poder eliminar un producto del sistema

#### Criterios de aceptación
**Escenario 1:** Administrador elimina un usuario 

- **Dado que** Administrador está en la pantalla de administración y ha buscado un producto
- **Cuando** Administrador ha pulsado el botón eliminar producto
- **Entonces** Se muestra mensaje de que el producto fue eliminado y se elimina de la base de datos 