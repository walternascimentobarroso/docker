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
