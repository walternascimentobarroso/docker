# Docker Hexo
Dockerfile para criar uma imagem do hexo

## Instalação
```bash
docker pull walternascimento/hexo
```

## Inicialização
```bash
docker run -d --name blog -p 4000:4000 \
	-v $(pwd):/root/blog \
	walternascimento/hexo
```
