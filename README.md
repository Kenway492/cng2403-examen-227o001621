# Examen práctico 2: Herramientas

## Objetivo del proyecto
Desplegar una aplicación web sencilla en tres servicios independientes con Docker Compose y gestionar su código con Git y GitHub.

## Imagen utilizada
`examen:227o001621`, construida a partir de `nginx:alpine` con el contenido de la carpeta `web/`.

## Puertos
| Servicio | Puerto en el equipo |
|----------|---------------------|
| web1     | 8081                |
| web2     | 8082                |
| web3     | 8083                |

## Cómo levantar los servicios
```bash
docker build -t examen:227o001621 .
docker compose up -d
docker compose ps
```