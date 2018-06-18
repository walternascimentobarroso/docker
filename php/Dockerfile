# Image and version
FROM php:7.2

# Maintainer
MAINTAINER walternascimentobarroso@gmail.com

# Install curl and php
RUN apt-get update -y
RUN apt-get install build-essential -y
RUN apt-get install curl git zip -y
RUN apt-get install libpng-dev -y

# Call PHP images script `docker-php-ext-install` and install language extensions
RUN docker-php-ext-install pdo_mysql gd

# Install composer
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer

# Change working dir
WORKDIR /code

# Port Export
EXPOSE 8080
