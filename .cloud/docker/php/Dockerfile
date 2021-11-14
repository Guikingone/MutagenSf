FROM php:7.4-fpm

WORKDIR /srv/app

RUN apt-get update -y && apt-get install -y git libzip-dev zip \
    && docker-php-ext-install zip

COPY --from=composer /usr/bin/composer /usr/bin/composer

EXPOSE 9000
