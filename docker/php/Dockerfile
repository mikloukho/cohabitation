FROM php:8.1-fpm

RUN apt-get update && apt-get install -y \
                        git \
                        wget \
                        unzip \
                        libpq-dev

RUN docker-php-ext-install pdo_pgsql

RUN wget https://getcomposer.org/installer -O - -q | php -- --install-dir=/bin --filename=composer --quiet

WORKDIR /var/www
