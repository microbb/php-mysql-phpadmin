FROM php:8.0.2-fpm

RUN apt-get update && apt-get install -y \
    git \
    curl \
    zip \
    unzip \
    libmariadb-dev

RUN docker-php-ext-install mysqli

COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer

WORKDIR /var/www


