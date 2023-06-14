# Ticket API

Este proyecto es una API construida con Laravel y MySQL que permite crear, eliminar, editar y recuperar tickets con paginación. Además, se puede obtener una lista de todos los tickets o filtrar por un ticket específico. Cada ticket tiene un ID, un usuario asociado, una fecha de creación, una fecha de actualización y un estado (abierto/cerrado).

## Requisitos

- PHP >= 7.4
- Composer
- MySQL

## Instalación

1. Clona el repositorio: 
``` git clone https://github.com/blommorflor/dvp-backend-1.git```

2. Instala las dependencias de Composer:
``` composer install ```

3. Copia el archivo de configuración .env.example

4. Configura la conexión a la base de datos en el archivo `.env`. Asegúrate de proporcionar los valores correctos para tu entorno

5. Ejecuta las migraciones para crear las tablas de la base de datos:

``` php artisa migrate ```

8. Inicia el servidor de desarrollo:

```php artisan serve ```


La API estará disponible en http://localhost:8000.

## Uso

La API ofrece los siguientes endpoints:

- **GET /api/tickets**: Recupera una lista paginada de todos los tickets.
- **GET /api/tickets/{id}**: Recupera un ticket específico por su ID.
- **POST /api/tickets**: Crea un nuevo ticket.
- **PUT /api/tickets/{id}**: Actualiza un ticket existente.
- **DELETE /api/tickets/{id}**: Elimina un ticket existente.

Para realizar peticiones a la API, puedes utilizar herramientas como cURL, Postman o cualquier cliente HTTP de tu elección.
