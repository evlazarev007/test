FROM php:8.2.10-apache

# Установка зависимостей
RUN apt-get update && apt-get install -y \
    libpng-dev \
    libjpeg-dev \
    libfreetype6-dev \
    && docker-php-ext-configure gd --with-freetype --with-jpeg \
    && docker-php-ext-install gd

# Установите другие необходимые PHP-расширения по мере необходимости

WORKDIR /var/www/html
