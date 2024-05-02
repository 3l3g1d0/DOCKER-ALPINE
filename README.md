# DOCKER-ALPINE

Este proyecto es un servidor Nginx básico usando Docker y Nginx.

## Requisitos

- Necesitas tener un docker instalado en tu máquina. Descargalo aqui [Docker](https://www.docker.com/get-started) con guías de instalación.

## Estructura del proyecto

- `Dockerfile`: Define la imagen Docker que instala Nginx en Alpine Linux.
- `nginx.conf`: Configuración principal de Nginx.
- `default.conf`: Configuración específica del servidor dentro de Nginx.

## Configuración de Nginx

`nginx.conf` y `default.conf` están configurados para servir contenido estático desde `/usr/share/nginx/html`. `nginx.conf` incluye también ajustes basicos y `events`.

## Uso

Para construir y ejecutar el contenedor Nginx:

```bash
docker build -t my-nginx .
docker run -p 80:80 my-nginx
