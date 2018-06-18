# Docker php
Dockerfile para criar uma imagem do PHP

## Instalação
```bash
docker build -t php-image .
```

## Inicialização
Se for a primeira inicialização:

```bash
docker run --name php-container -it --privileged -p 8080:8080 -v ~/projetos:/code php-image bash
```

Se não for a primeira

```bash
docker start php-container
docker exec -it php-container bash
```

Caso queira executar o servidor do php:

```bash
php -S 0.0.0.0:8080
```

### Executar o projeto no browser
[http://localhost:8080/](http://localhost:8080/ "Exibi o projeto")


## Mudar permissão
Se algum arquivo foi criado pelo usuario do container(root), você pode modificar para editar fora do container:

```bash
sudo chown <usuario.grupo> -R <pastadoprojeto>
```

