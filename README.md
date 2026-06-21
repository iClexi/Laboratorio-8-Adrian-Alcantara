<div align="center">

# Laboratorio 8 - Docker, Portainer y WordPress

### Practicas de contenedores en Ubuntu Server usando Docker, Portainer y Docker Compose.

![Platform](https://img.shields.io/badge/Platform-Ubuntu%20Server-E95420?logo=ubuntu&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Engine-2496ED?logo=docker&logoColor=white)
![Portainer](https://img.shields.io/badge/Portainer-Management-blue)
![Compose](https://img.shields.io/badge/Docker%20Compose-WordPress-green)
![Topic](https://img.shields.io/badge/Topic-Containers-purple)

</div>

---

## Descripcion

Este laboratorio introduce la administracion de contenedores en Ubuntu Server. Incluye instalacion de Docker Engine, despliegue de Portainer para administracion visual y publicacion de WordPress usando Docker Compose con base de datos MySQL.

## Practicas incluidas

| Practica | Tema | Objetivo |
| --- | --- | --- |
| Practica 1 | Docker + NGINX | Instalar Docker y ejecutar un contenedor web |
| Practica 2 | Portainer | Administrar Docker desde una interfaz web |
| Practica 3 | WordPress | Desplegar WordPress con Docker Compose |

## How-To: usar el laboratorio

1. Prepara una VM Ubuntu Server.
2. Instala Docker desde el repositorio oficial.
3. Verifica Docker con `docker version` y un contenedor de prueba.
4. Despliega Portainer para administrar contenedores.
5. Usa Docker Compose para levantar WordPress y MySQL.

## Requisitos

- Ubuntu Server.
- Acceso `sudo`.
- Internet para descargar imagenes.
- Puertos disponibles para NGINX, Portainer y WordPress.

## Comandos clave

```bash
sudo apt update
sudo apt install -y ca-certificates curl gnupg lsb-release
sudo systemctl enable --now docker
sudo docker version
sudo docker run -d -p 80:80 nginx
sudo docker volume create portainer_data
docker-compose up -d
```

## Estructura del repositorio

```text
Laboratorio-8-Adrian-Alcantara/
├── Practica 1 - Instalacion y configuracion de Docker
├── Practica 2 - Instalacion de Portainer
├── Practica 3 - Despliegue de contenedor de Wordpress utilizando Docker-Compose
└── README.md
```

## Resultado esperado

Al terminar, el estudiante debe poder instalar Docker, administrar contenedores con Portainer y desplegar una aplicacion completa de WordPress usando Docker Compose.
