docker build -t ionic .

docker run --name ionic -it --privileged -p 8100:8100 -v ~/projetos:/www/app ionic bash

docker exec -it ionic bash

sudo chown <usuario.grupo> -R <pastadoprojeto>

aplicação:
http://localhost:8100/



# Docker Ionic
Dockerfile para criar uma imagem do Ionic

## Instalação
```bash
docker pull walternascimento/ionic
```

## Inicialização
```bash
docker run -d --name app -p 4000:4000 \
	-v $(pwd):/root/app \
	walternascimento/ionic
```

