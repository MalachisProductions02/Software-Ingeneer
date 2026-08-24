# Desarrollar una aplicación para la Universidad Modelo

La aplicación será para comprar cosas en la tiendita por medio de pedidos en linea y solo pasar a recoger asi evitamos el tiempo de espera que se genera en los descansos para comprar físicamente la comida.

La aplicación funcionará en cualquier plataforma siendo dispositivos móviles la prioritaria.

Se contará con un inicio de sesión gestionadio con ```MySQL``` para poder almacenar estos datos.

Tanto los alumnos como los profesores podrán iniciar sesión y para corroborar que sean de la escuela, se verificará con su matrícula y correo institucional.

La arquitectura del proyecto se piensa construir mediante uso de ```Python Flask``` en conjunto con un esqueleto hecho con ```HTML```, ```CSS``` para diseño y ```JavaScript``` para animaciones sofisticadas y adornar el proyecto.

La aplicación mostrará un menú virtual de todo el contenido de las cafeterías y los separá respecto a la ubicación de cada cafetería, además, al comprar, te preguntará dónde quieres recoger tu pedido para mayor control.

Al realizar una compra se usarán APIs de PayPal para gestionar compras en línea y cuando se realice una entonces se crea un token virtual el cual llegará a la sesión de administrador que lo podrán ver los empleados de la cafetería para poder realizar la orden.

El token contará con los siguientes datos:

- Nombre del Alumno/Profesor
- Cafetería para recolección
- Monto Pagado
- Nombre del Producto
- Token generado en hexadecimal de 8 dígitos como identificador

Será hosteado mediante un servidor en línea y se utilizará **GitHub** para el control de _Backups_ trabajado desde un _ambiente virtual_ parar evitar dañar la Rama Priincipal del proyecto.