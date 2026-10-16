# API CRUD de personas

API REST con Node.js, Express y MySQL/MariaDB. Se conecta a la base de datos `proyecto` y administra la tabla `personas` (`id`, `nombre`).

## Configuración

1. Instala Node.js y MySQL/MariaDB.
2. Ejecuta `schema.sql` en el servidor de base de datos para crear la base y la tabla (si ya existen, no se reemplazan).
3. Copia `.env.example` a `.env` y configura el host, usuario y contraseña de MySQL. No compartas ni subas el archivo `.env`.
4. Ejecuta `npm install` y luego `npm start`.

El servidor inicia en `http://localhost:3000` (se puede cambiar con `PORT`).

## Rutas

| Método | Ruta | Acción |
| --- | --- | --- |
| GET | `/api/personas` | Listar personas |
| GET | `/api/personas/:id` | Obtener una persona |
| POST | `/api/personas` | Crear una persona; JSON: `{"nombre":"Ana"}` |
| PUT | `/api/personas/:id` | Actualizar el nombre; JSON: `{"nombre":"Ana López"}` |
| DELETE | `/api/personas/:id` | Eliminar una persona |
