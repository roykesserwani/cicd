FROM php:7.2-fpm
MAINTAINER Roy Kesserwani <roy@infonyze.com>
WORKDIR /var/www/html

RUN apt-get update && apt-get install -y zlib1g-dev libpng-dev libpcre3-dev
RUN apt-get install nano
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
RUN docker-php-ext-install zip gd pdo_mysql