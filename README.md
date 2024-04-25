# Kit básico de inicio de Docker
Sitio básico para instalar apps de php, ideal para realizar pruebas, soltar la mano.

Se ha usado como base el repositorio de [refactorian](https://github.com/refactorian) / [laravel-docker](https://github.com/refactorian/laravel-docker)


## Kit de inicio de Docker
- PHP v8.2.x
- MySQL v8.3.x (default)
- phpMyAdmin v5.x
- Mailpit v1.x
- Node.js v18.x
- NPM v10.x
- Yarn v1.x
- Vite v5.x
- Rector v1.x
- Redis v7.2.x

## Requerimientos
- Versión estable de [Docker](https://docs.docker.com/engine/install/)
- Versión compatible de [Docker Compose](https://docs.docker.com/compose/install/#install-compose)

## ¿Cómo implementar?

### ¡Solo por primera vez!
- `git clone https://github.com/jfuentes3002/docker-php82-basico.git php82`
- `cd php82`
- `docker compose up -d --build`
- `docker compose exec php bash`
- `composer setup`

### A partir de la segunda vez
- `docker compose up -d`

## Notas

### App
- URL: http://localhost

### Mailpit
- URL: http://localhost:8025

### phpMyAdmin
- URL: http://localhost:8080
- Server: `mysql`
- Username: `refactorian`
- Password: `refactorian`
- Database: `refactorian`

### Adminer
- URL: http://localhost:9090
- Server: `mysql`
- Username: `refactorian`
- Password: `refactorian`
- Database: `refactorian`

### Comandos básicos de docker compose
- Construir o re-construir servicios
    - `docker compose build`
- Crear e iniciar contenedores
    - `docker compose up -d`
- Detener y eliminar contenedores, redes.
    - `docker compose down`
- Detener todos los servicios
    - `docker compose stop`
- Reiniciar servicio de contenedores
    - `docker compose restart`
- Ejecutar un comando dentro de un contenedor
    - `docker compose exec [container] [command]`

