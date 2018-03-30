FROM node:latest

MAINTAINER "Walter Nascimento <walternascimentobarroso@gmail.com>"

WORKDIR /www/app

# Install JAVA(openJDK)
RUN	echo "deb http://http.debian.net/debian jessie-backports main" | \
	tee --append /etc/apt/sources.list.d/jessie-backports.list > /dev/null && \
	apt-get update && \
	apt-get install -y -t jessie-backports openjdk-8-jdk

# Install GIT
RUN	apt-get install -y git && \
	git config --global user.email "walternascimentobarroso@gmail.com" && \
	git config --global user.name "Walter Nascimento Barroso" 

# Install unzip
RUN	apt-get install -y unzip

# Install IONIC and CORDOVA
RUN	npm install -g cordova ionic

# Download and Extraction GRADLE
RUN	wget https://downloads.gradle.org/distributions/gradle-4.6-bin.zip
	unzip gradle-4.6-bin.zip -d /opt/gradle/

# Setup environment GRADLE
ENV GRADLE_HOME /opt/gradle/gradle-4.6
ENV PATH ${PATH}:${GRADLE_HOME}/bin

# Download and Extraction ANDROID-SDK
RUN	wget https://dl.google.com/android/repository/sdk-tools-linux-3859397.zip &&\
	unzip sdk-tools-linux-3859397.zip -d /opt/android-sdk/

# Setup environment ANDROID
ENV ANDROID_HOME /opt/android-sdk
ENV PATH ${PATH}:${ANDROID_HOME}/tools:${ANDROID_HOME}/platform-tools

# Expose port: web (8100), livereload (35729)
EXPOSE 8100 35729
