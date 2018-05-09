# Docker Angular
Dockerfile para criar uma imagem do Angular

## Instalação
```bash
docker pull walternascimento/angular
```

## Inicialização
```bash
docker run -d --name app -p 4200:4200 \
	-v $(pwd):/root/app \
	walternascimento/angular
```



docker build -t angular .

docker run --name angular -it --privileged -p 4200:4200 -v ~/projetos:/www/app angular bash

docker exec -it angular bash

sudo chown <usuario.grupo> -R <pastadoprojeto>

ng serve --host 0.0.0.0

aplicação:
http://localhost:4200/

