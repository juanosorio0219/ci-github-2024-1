# Proyecto CI/CD con Docker y GitHub Actions
Este proyecto es un ejemplo de cómo construir, subir y automatizar la gestión de imágenes Docker utilizando GitHub Actions y Docker Hub.

## Descripción del Proyecto
El objetivo de este proyecto es construir una imagen Docker para un proyecto React, subirla a Docker Hub y automatizar el proceso con un pipeline de GitHub Actions.

## Configuración de Docker
Para construir y subir la imagen Docker, necesitas tener Docker instalado y configurado en tu entorno local.

## Construcción de la Imagen Docker
Para construir la imagen Docker del proyecto React, utiliza el siguiente comando:

```bash
docker build -t <nombre-de-la-imagen> .
```

## Configuración de GitHub Actions
Para automatizar la construcción y subida de la imagen Docker, se usó un archivo YAML que define el flujo de trabajo. Este archivo debe estar en la carpeta .github/workflows/ de tu repositorio.

## Configuración de Secretos
Para usar este pipeline, debes configurar secretos en GitHub para tu repositorio:

DOCKER_USERNAME: Tu nombre de usuario de Docker Hub.
DOCKER_PASSWORD: El Personal Access Token con permisos para subir a Docker Hub.
Para agregar secretos, ve a la configuración de tu repositorio en GitHub, busca la sección "Secrets and variables", y agrega los secretos necesarios.

## Uso del Pipeline
Una vez configurado el pipeline, este se ejecutará cada vez que hagas un "push" a la rama "main". Puedes monitorear el progreso del pipeline desde la pestaña "Actions" en GitHub.
<img width="1437" alt="Screenshot 2024-04-23 at 7 56 29 PM" src="https://github.com/juanosorio0219/ci-github-2024-1/assets/80568091/bf350d63-1287-46b2-b694-9baed5e30359">

## Verificación de la Imagen en Docker Hub
Una vez que hayas subido la imagen a Docker Hub, puedes verificar que se haya subido correctamente

<img width="791" alt="Screenshot 2024-04-23 at 7 58 51 PM" src="https://github.com/juanosorio0219/ci-github-2024-1/assets/80568091/0a5dae8a-8ca8-441b-801c-c9b7d0b803b6">
