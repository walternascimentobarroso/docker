# Docker php
Dockerfile para criar uma imagem do PHP

## Instalação
```bash
docker pull walternascimento/php
```

## Inicialização
```bash
docker run -d --name app -p 8080:8080 \
	-v $(pwd):/root/app \
	walternascimento/php
```



docker build -t php .

docker run --name php -it --privileged -p 8080:8080 -v ~/projetos:/www/app php bash

docker exec -it php bash

sudo chown <usuario.grupo> -R <pastadoprojeto>

php -S localhost:8080 

aplicação:
http://localhost:8080/

