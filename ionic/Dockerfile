FROM node:latest

MAINTAINER "Walter Nascimento <walternascimentobarroso@gmail.com>"

WORKDIR /www/app

# Install JAVA(OpenJDK)
RUN	add-apt-repository ppa:openjdk-r/ppa && \
	apt-get update && \
	apt-get install software-properties-common && \
	apt-get install -y \
	openjdk-8-jdk

# Install GIT
RUN	apt-get install -y git && \
	git config --global user.email "walternascimentobarroso@gmail.com" && \
	git config --global user.name "Walter Nascimento" 

# Install IONIC and CORDOVA
RUN	npm install -g cordova ionic

# Download and Extraction ANDROID-SDK
RUN	wget https://dl.google.com/android/repository/sdk-tools-linux-3859397.zip &&\
	unzip sdk-tools-linux-3859397.zip /opt/android-sdk/

# Expose port: web (8100), livereload (35729)
EXPOSE 8100 35729
