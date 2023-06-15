# Projeto Integrador II B

## Instalação do Docker

    sudo curl -fsSL https://get.docker.com -o get-docker.sh
    sudo sh ./get-docker.sh

## Subindo Aplicação no Docker Compose

    cd /opt/ && nano docker-compose.yml
    docker compose up -d
  
## Definição do docker-compose.yml

    version: '3.1'
    
    services:
    
      webapp:
        image: galactros/integration-project-webapp:latest
        container_name: webapp
        ports:
          - "80:80"

## Acessando a aplicação

Basta acessar no navegador com o **IP** onde foi instalado a aplicação.
**Ex:** localhost
