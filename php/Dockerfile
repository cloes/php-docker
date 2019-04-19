FROM php:7.2-fpm

RUN docker-php-ext-install mysqli

RUN sed -i s/deb.debian.org/mirrors.163.com/g /etc/apt/sources.list /etc/apt/sources.list.d/buster.list
RUN sed -i s/security.debian.org/mirrors.163.com/g /etc/apt/sources.list /etc/apt/sources.list.d/buster.list

RUN apt-get update && apt-get install -y apt-utils
RUN apt-get install -y procps

RUN mkdir /code

RUN chown -R www-data /code
