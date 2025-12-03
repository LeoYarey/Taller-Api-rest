# Taller: API REST con Node.js y Express

Proyecto práctico para validar conocimientos sobre la creación de servicios RESTful utilizando Node.js. Este servidor permite gestionar un CRUD básico de usuarios en memoria.

## Descripción
Esta API proporciona endpoints para consultar, crear, actualizar y eliminar usuarios utilizando los verbos HTTP estándar. Fue desarrollada como parte del taller de "APIs REST".

## Tecnologías Utilizadas
* Node.js: Entorno de ejecución.
* Express: Framework web para el manejo de rutas y middlewares.
* Nodemon: Herramienta de desarrollo para reinicio automático.

## Instalación y Ejecución

Sigue estos pasos para correr el proyecto en tu entorno local:

1. Instalar dependencias:
    Asegúrate de estar en la carpeta del proyecto y ejecuta:
    ```bash
    npm install
    ```

2. Ejecutar el servidor (Modo Desarrollo):
    El proyecto cuenta con un script configurado para usar `nodemon`:
    ```bash
    npm run dev
    ```
    El servidor iniciará en: `http://localhost:3000`

## Endpoints Disponibles

La API cuenta con los siguientes recursos:

| Método | Ruta | Descripción | Cuerpo (Body) Requerido |
| :--- | :--- | :--- | :--- |
| GET | `/` | Mensaje de bienvenida. | N/A |
| GET | `/saludo` | Retorna un JSON con saludo y fecha. | N/A |
| GET | `/user` | Lista todos los usuarios. | N/A |
| POST | `/user` | Crea un nuevo usuario. | `{ "nombre": "...", "edad": 0 }` |
| PUT | `/user/:id` | Actualiza un usuario existente. | `{ "nombre": "...", "edad": 0 }` |
| DELETE | `/user/:id` | Elimina un usuario por ID. | N/A |

## Pruebas
Puedes probar los endpoints utilizando Thunder Client (VS Code), Postman o cualquier cliente HTTP.

---
**Autor:** [Tu Nombre]
**Materia:** Taller REST NODEJS
