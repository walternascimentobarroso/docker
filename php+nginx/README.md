# Docker php

docker-compose para criar uma imagem com PHP e NGINX

## Instalação

```bash
docker-compose up
```

## Inicialização

Se for a primeira inicialização:

```bash
docker-compose up --build
```

Se não for a primeira

```bash
docker-compose up -d
```

### Executar o projeto no browser

[http://localhost:80/](http://localhost:80/ "Exibi o projeto")

### Acessar o conteiner

Caso queira acessar algum conteiner basta executar o comando abaixo:

```bash
docker exec -it php_crud bash
```
