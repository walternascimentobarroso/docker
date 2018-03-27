FROM node:latest

WORKDIR /www/app

RUN apt-get update && \
    npm install -g cordova ionic && \
    apt-get install -y git && \
    git config --global user.email "walternascimentobarroso@gmail.com" && \
    git config --global user.name "Walter Nascimento"

EXPOSE 8100 4200 35729
