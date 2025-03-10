# Gestor de tareas

El objetivo de este proyecto es crear un servidor en Node usando **ExpressJS** con el fin de que los estudiantes practiquen la lógica del servidor. El servidor debe manejar una base de datos **SQLite** y debe contar con validación de datos adecuada.

Este ejercicio está diseñado específicamente para que los estudiantes adquieran experiencia en la implementación de funcionalidades del servidor utilizando **NodeJS** y **Express**.

## Endpoints esperados

- **GET /app**: En este endpoint se despliega un cliente básico que se va a comunicar con el servidor. Puede ser hecho con cualquier tecnología web como **React**, **HTML puro**, **Vue** o cualquier otra, siempre y cuando al acceder al servidor en la ruta **/app** se pueda visualizar el cliente.

- **GET /tasks**: Este endpoint retornará todas las tareas almacenadas en la base de datos.

- **POST /task**: Este endpoint permite agregar una nueva tarea a la base de datos. Debe recibir un JSON con los datos necesarios para agregar una tarea, asegurándose de incluir validación para verificar que todos los campos requeridos estén presentes y en el formato adecuado.

- **GET /task/:id**: Este endpoint retorna una tarea específica con base en su ID.

- **PUT /task/:id**: Este endpoint permite actualizar una tarea existente identificada por su ID. Debe recibir un JSON con los campos que se deseen actualizar, asegurándose de que los campos requeridos estén presentes y en el formato adecuado.

- **DELETE /task/:id**: Este endpoint permite eliminar una tarea específica por su ID.

## Requisitos mínimos del modelo "task" en la base de datos
- **id**: Integer, clave primaria, autoincrementable.
- **title**: String, requerido.
- **description**: String, opcional.
- **status**: String, valores permitidos **["pending", "completed"]**, requerido.
- **createdAt**: Date, fecha de creación, generado automáticamente.
- **updatedAt**: Date, fecha de última actualización, generado automáticamente.# Gestor de tareas
