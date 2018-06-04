FROM php:7.2

MAINTAINER walternascimentobarroso@gmail.com

WORKDIR /www/app

RUN	apt-get update && \
	php -r "readfile('http://getcomposer.org/installer');" | php -- --install-dir=/usr/bin/ --filename=composer

EXPOSE 8080
