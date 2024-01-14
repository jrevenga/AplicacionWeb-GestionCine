# Aplicación Web Gestión de Cine
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/6c39fdad-8d99-4225-89fc-a38e3c616b58)

Este proyecto web se centra en la creación de una aplicación cliente/servidor utilizando el patrón de diseño Modelo Vista Controlador (MVC). Se han incorporado diversas herramientas y tecnologías a lo largo de la asignatura, cumpliendo con los siguientes requisitos:

## Tecnologías Utilizadas

- **Frontend**:
  - HTML5
  - CSS3
  - JavaScript (jQuery)

- **Backend**:
  - Java (implementando el patrón MVC)
  - Servlets para gestionar las solicitudes HTTP y coordinar las respuestas.
  - Páginas JSP para la representación de las vistas y la interacción con el usuario.
  - DAO (Data Access Object) para interactuar con la base de datos.

- **Autenticación y Sesiones**:
  - Implementación de autenticación y sesiones para garantizar la seguridad y gestión de usuarios.

- **Almacenamiento de Datos**:
  - Apache Derby se utiliza como sistema de gestión de base de datos para el almacenamiento de información relacionada con películas, salas, entradas, etc.

## Estructura de Archivos

- **Proyecto Java**: Desarrollado en NeatBeans, contiene la lógica de la aplicación siguiendo el patrón MVC.

- **model.sql**: Archivo SQL que crea las tablas de la base de datos.

- **datos.sql**: Archivo SQL que contiene datos para rellenar las tablas de la base de datos.

- **Database.png**: Imagen del diagrama UML de la base de datos, proporcionando una visualización clara de la estructura.

- **memoria.pdf**: Documento detallado que describe la aplicación en profundidad, incluyendo un manual de usuario para una mejor comprensión y utilización.

## Esquema de Información y Modelo E/R

El sistema se basa en un esquema de información que incluye:
- **Películas**: Con detalles como nombre, sinopsis, página oficial, título original, género, nacionalidad, duración, año, distribuidora, director, actores, clasificación por edad y otros datos de interés.
- **Salas**: Con información sobre el nombre de la sala, filas y columnas.
- **Entradas**: Permite ver una película en una sala en una fecha y hora específicas, con detalles como fila, columna y nombre de la película.

## Funcionalidades de la Administración/Gestión

La parte administrativa requiere autenticación y validación de sesión para gestionar diversos aspectos del cine. Las funcionalidades incluyen:

- **Gestión de Películas**: Insertar, borrar, modificar y consultar información sobre películas.
- **Gestión de Salas**: Insertar, borrar, modificar y consultar detalles sobre las salas.
- **Gestión de Entradas**: Insertar, borrar, modificar y consultar información sobre las entradas.
- **Gestión de Reservas**: Consultar reservas realizadas por los clientes.
- **Gestión de Informes**: Generar listados de películas por género, salas, etc.

## Funcionalidades para los Clientes

La interfaz para los clientes proporciona acceso a la web de la compañía con información sobre películas y otros contenidos. Las funcionalidades para los clientes incluyen:

- **Registro**: Los clientes pueden registrarse para realizar reservas y dejar comentarios sobre las películas.
  
- **Reserva**: Posibilidad de reservar entradas de cine desde la web. Después de autenticarse y validar la sesión, el cliente puede seleccionar película, día, hora y sala. Se mostrará una representación gráfica de la sala para elegir los asientos y se solicitará un número de tarjeta para realizar el pago. Si la reserva es exitosa, se proporcionará al cliente un número de referencia.

- **Comentarios**: Los usuarios registrados pueden ver y agregar comentarios sobre las películas. Esto incluye valoraciones proporcionadas por otros usuarios.


# Manual de Usuario

## Ventana Principal

La ventana principal ofrece acceso a diferentes secciones, como "Inicio" y la lista de películas, a través de las listas en la parte izquierda del encabezado. En la parte derecha, encontrarás un botón de ayuda (simulado como un marcador de posición) y botones para iniciar sesión o registrarte. Al hacer clic en los títulos de las películas, puedes acceder directamente a la información de la película.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/03dc8951-0829-48ba-b406-308e9ca66024)

Más abajo, se encuentran los trailers de las películas y el pie de página con enlaces de marcador de posición para simular enlaces típicos de una página web.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/b6ee8709-9114-49e4-aa1d-632d4a450517)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/bd3bdc0d-8227-43ea-b7c5-9d92a8dccf07)

## Registro

Al hacer clic en el botón de registro, se abrirá una ventana que te permitirá crear un usuario para acceder a funcionalidades exclusivas.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/094ca559-270a-4c82-ab6a-19e6d68e39a2)

## Inicio de Sesión

El botón de inicio de sesión te lleva a una ventana donde puedes iniciar sesión como administrador o cliente. Para este ejemplo, iniciaremos sesión como cliente.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/4f3bb662-4a97-40c8-9386-4d9821b14f6e)

## Lista de Películas

Al hacer clic en la lista de películas, se mostrará una ventana que te permite seleccionar cualquier película que se proyecte en el cine.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/38053305-ca00-43bb-b630-7e12d7728ee2)

## Información de Película

Al hacer clic en una película, se muestra información básica sobre la misma. Si estás autenticado como usuario, también podrás ver y dejar comentarios.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/c658cb86-2b41-47ca-ba71-b3361c54fff4)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/b03d4a4d-469f-45c4-9d51-056afde6c125)

## Reserva de Entradas

Si decides reservar entradas, podrás ver las salas donde se proyecta la película, la información de las proyecciones y, al seleccionar "Ver Asientos", podrás elegir los asientos disponibles.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/41126c45-c3b2-4e3f-9746-6e33fe07631d)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/f409c1b9-695d-4c66-a8ff-95471ecda168)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/fd99ad36-0056-46bb-9b10-57d85658c75c)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/d975f260-a1fc-405c-8e06-716c66a7f7a3)

## Confirmación de Reserva

Después de seleccionar los asientos y confirmar la reserva, se mostrará el número de reserva y un botón para volver al inicio.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/166664b5-d957-4715-b0c6-426ec4a3c89c)

## Funcionalidades del Administrador

Inicia sesión como administrador con el usuario "admin@admin.com" y la contraseña "12345". Desde la ventana principal, puedes cerrar sesión, gestionar películas, salas, proyecciones, reservas e informes.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/7aa574fe-0bc3-42f3-8c31-f7c3c9a041fa)

## Gestión de Películas

En la sección de gestionar películas, puedes ver, crear, editar y eliminar películas. Al crear o editar, se abrirán ventanas para ingresar o modificar información.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/40c76063-1d19-444d-899f-b1a3114e1419)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/e338ea8a-412e-4876-918d-90c7cafd21aa)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/a9db79a8-f9a4-4bda-94cc-ec01b7877ee8)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/bd7f4d4b-47c9-46d2-8f39-6aaa5def763b)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/051304f5-d44c-45f8-bcd3-a307c2415adc)

## Gestión de Salas

Similar a la gestión de películas, puedes ver, crear, editar y eliminar salas.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/b150158d-7c82-490c-9091-1a159d406f6c)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/1b335880-b63e-4ed1-988a-4146faf17ce8)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/d8112536-eead-4d14-9963-5f9517a0c067)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/dff85ef9-c87c-4cb4-8ae6-eefee6ea250a)

## Gestión de Proyecciones

Esta sección permite gestionar proyecciones. Puedes crear, editar y eliminar proyecciones. También puedes gestionar las entradas de una proyección específica.

## Gestionar Reservas

Aquí puedes ver todas las reservas realizadas, incluyendo detalles como el número de tarjeta y el número de referencia.

## Gestionar Informes

La sección de informes proporciona información sobre películas ordenadas por género y otros datos importantes.
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/b52966bd-c64d-4463-b86c-c4116599cb5c)
![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/ab75111c-9b5f-4af6-8110-f892845183c0)

Este resumen proporciona una visión general de las funcionalidades de la aplicación. Para obtener más detalles y explicaciones paso a paso, consulta el documento completo adjunto en el archivo PDF "memoria.pdf".


 
