FROM php:8.0-fpm

RUN apt-get update

RUN apt-get install -y git zip unzip curl libzip-dev

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# RUN docker-php-ext-configure zip --with-libzip

RUN docker-php-ext-install pdo_mysql zip
