![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/1c7dfca5-bf46-497f-8a6c-9b23897b34c5)# Aplicación Web Gestión de Cine

![image](https://github.com/jrevenga/AplicacionWeb-GestionCine/assets/124138100/3f689e9b-a486-4ce0-a239-b6f3aa6a6fc9)

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

**Nota: Se han utilizado Servlets, páginas JSP, DAO, entre otras tecnologías para la implementación efectiva de la aplicación. Se mantendrán sesiones de forma obligatoria para gestionar la información de cada cliente de manera independiente.**

 
