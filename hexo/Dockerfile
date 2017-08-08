FROM node:7.1

MAINTAINER walternascimentobarroso@gmail.com

WORKDIR /root

RUN \
  npm config set registry https://registry.npm.taobao.org/ && \
  mkdir blog && cd blog && \
  npm install hexo-cli -g


WORKDIR /root/blog/

VOLUME ["/root/blog/"]

EXPOSE 4000

CMD ["hexo", "server", "-i", "0.0.0.0"]
