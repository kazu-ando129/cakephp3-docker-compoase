FROM php:7.2.17-fpm-stretch

RUN apt-get update && \
    apt-get install -y libicu-dev && \
    docker-php-ext-install intl pdo_mysql

WORKDIR /var/www/html