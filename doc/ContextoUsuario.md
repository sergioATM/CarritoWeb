# Contexto Usuario

## Características
Usuario que se ha registrado en el sistema y que por lo tanto sus datos están en nuestra base de datos. Estos usuarios podrán realizar todas las funciones de un usuario anónimo y ademas podrán efectuar y finalizar las compras añadidas al carrito de la compra.

## Escenarios como Usuario

### Escenario loggearse
##### Usuario para hacer un login correcto deberá introducir su dirección de correo y su contraseña
+ **Como** Usuario
+ **Quiero** Hacer login
+ **Para** Acceder a la web bajo mi perfil 
#### Criterio de aceptación 

 **Escenario 1:** Usuario hace un login incorrecto

- **Dado que** Usuario ha introducido un correo electrónico o una contraseña que no corresponden con  los datos registrados en la base de datos
- **Cuando** Usuario ha pulsado el botón entrar
- **Entonces** Se muestra mensaje de error informando que algún dato no es correcto y se recarga la pagina de login

 **Escenario 2:** Usuario hace login correctamente

- **Dado que** Usuario ha introducido un correo electrónico y una contraseña que corresponden con los datos registrados en la base de datos
- **Cuando** Usuario ha pulsado el botón entrar
- **Entonces** Se valida usuario y se muestra pagina principal y dentro de pagina principal se muestra el menú  de usuario 

### Escenario cambiar contraseña

##### Usuario para cambiar la contraseña con éxito deberá introducir una nueva contraseña de más de 6 caracteres y que no sea similar a la anterior

+ **Como** Usuario
+ **Quiero** Cambiar contraseña
+ **Para** Tener la posibilidad de modificar su contraseña

#### Criterios de aceptación 

 **Escenario 1:** Usuario introduce nueva contraseña igual que la anterior

- **Dado que** Usuario ha introducido una contraseña similar a la anterior que no corresponde con los requisitos del sistema que son mínimo 6 caracteres y no puede ser igual que la anterior
- **Cuando** Usuario ha pulsado el botón cambiar contraseña
- **Entonces** Se muestra mensaje de error informando que la contraseña nueva no puede ser igual a la anterior y se recarga la pagina de cambiar contraseña

 **Escenario 2:** Usuario no introduce un formato correcto de nueva contraseña

- **Dado que** Usuario ha introducido una nueva contraseña de un formato que no corresponde con los requisitos del sistema que son mínimo 6 caracteres y no puede ser igual que la anterior
- **Cuando** Usuario ha ha pulsado el botón cambiar contraseña
- **Entonces** Se muestra mensaje de error informando que la contraseña nueva no puede ser inferior a 6 caracteres y se recarga la pagina de cambiar contraseña

 **Escenario 3:** Usuario introduce una nueva contraseña válida 

- **Dado que** Usuario ha introducido una nueva contraseña que corresponde con los requisitos del sistema que son mínimo 6 caracteres y no puede ser igual que la anterior
- **Cuando** Usuario ha pulsado el botón cambiar contraseña
- **Entonces** Se muestra mensaje informando que la contraseña ha sido cambiada con éxito y te redirige a la página principal de usuario y  nueva contraseña se guarda en la base de datos

### Escenario cerrar sesión
+ **Como** Usuario
+ **Quiero** Cerrar sesión
+ **Para** Cerrar la sesión de usuario actual
#### Criterio de aceptación 

 **Escenario 1:** Usuario cierra sesión

- **Dado que** Usuario ha cerrado sesión
- **Cuando** Usuario ha pulsado el botón cerrar sesión
- **Entonces** Se muestra mensaje de informando que usuario con nombre [] ha cerrado la sesión correctamente y te redirige a la pagina principal para usuarios anónimos

### Escenario modificar datos
##### Usuario para modificar los datos con éxito deberá rellenar todos los campos de texto
+ **Como** Usuario
+ **Quiero** Cambiar datos de la cuenta 
+ **Para** Cambiar datos como el e-mail, nombre, apellidos, dirección y todos los datos personales necesarios para el registro
#### Criterios de aceptación
 **Escenario 1:** Usuario deja un campo vacío

- **Dado que** Usuario ha dejado uno o mas campos del formulario sin información
- **Cuando** Usuario ha pulsado el botón modificar datos
- **Entonces** Se muestra mensaje de informando que no puede dejar ningún campo de texto de información

**Escenario 2:** Usuario cambia los datos correctamente

- **Dado que** Usuario ha rellenado todos los campos de texto
- **Cuando** Usuario ha pulsado el botón modificar datos
- **Entonces** Se muestra mensaje de informando que los datos han sido cambiados con éxito y se guardan en la base de datos
### Escenario añadir productos al carrito
##### Usuario para poder añadir productos al carrito tiene la posibilidad de modificar la cantidad de productos, pero por defecto viene 1 y no se podrá seleccionar 0. 
+ **Como** Usuario
+ **Quiero** Añadir productos al carrito
+ **Para** Tener todos los productos en el carrito y se pueda calcular su importe total
#### Criterio de aceptación
**Escenario 1:** Usuario añade una cantidad x de un producto al carrito

- **Dado que** Usuario ha seleccionado un producto y una cantidad 
- **Cuando** Usuario ha pulsado el botón añadir al carrito
- **Entonces** Se muestra mensaje de informando que los productos han sido añadidos con éxito y los productos se añaden al carrito

### Escenario modificar cantidad de un producto añadido al carrito
##### Usuario dentro del carrito se le muestra la cantidad y podrá modificarla además aparecerá una x para cancelar el producto total
+ **Como** Usuario
+ **Quiero** modificar cantidad de productos del carrito
+ **Para** Poder cambiar la cantidad de productos añadidos al carrito anteriormente
#### Criterio de aceptación

**Escenario 1:** Usuario modifica una cantidad de un producto añadido al carrito

- **Dado que** Usuario esta en el carrito y quiere modificar la cantidad de un producto
- **Cuando** Usuario ha modificado la cantidad
- **Entonces** Se muestra mensaje de informando que se ha cambiado la cantidad de productos y se modifica la cantidad

**Escenario 2:** Usuario elimina un producto total añadido al carrito

- **Dado que** Usuario esta en el carrito y quiere eliminar un producto
- **Cuando** Usuario ha pulsado el botón con la X
- **Entonces** Se elimina el producto total del carrito 

### Escenario ver carrito
+ **Como** Usuario
+ **Quiero** Ver los productos añadidos al carrito
+ **Para** Poder ver los productos añadidos al carrito y poder pasar a finalizar compra o a modificar algún producto
#### Criterio de aceptación 

**Escenario 1:** Usuario accede a ver los productos guardados en el carrito

- **Dado que** Usuario esta en cualquier parte de la pagina y quiere ver su carrito
- **Cuando** Usuario ha pulsado botón ver carrito
- **Entonces** Se muestra pagina de carrito con los productos guardados

### Escenario pagar y finalizar compra
+ **Como** Usuario
+ **Quiero** Pagar y finalizar compra
+ **Para** Poder finalizar la compra de los productos añadidos al carrito, procesar el pago y obtener una venta
#### Criterio de aceptación 

**Escenario 1:** Usuario quiere finalizar compra

- **Dado que** Usuario esta en el carrito y quiere finalizar la compra
- **Cuando** Usuario ha pulsado botón finalizar compra
- **Entonces** Se muestra pagina de pago para finalizar la compra 


