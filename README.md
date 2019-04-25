# Docker-frontend-env

## Building the image

docker build -f Dockerfile.dev -t docker-frontend-env .

## Creating a container

docker run -p 4200:4200 -v /app/node_modules -v $(pwd):/app docker-frontend-env

### Windows

docker run -p 4200:4200 -v /app/node_modules -v %cd%:/app docker-frontend-env

## Running with docker-compose

docker-compose up
