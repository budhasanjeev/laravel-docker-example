FROM php:8.2-fpm

RUN apt-get update -y

# Installs system dependencies
RUN apt-get install -y zlib1g-dev vim libzip-dev

# Installs PHP extensions
RUN docker-php-ext-install zip pdo_mysql

# Get from composer container and copy to current container
COPY --from=composer:2.6 /usr/bin/composer /usr/bin/composer

WORKDIR /var/www
