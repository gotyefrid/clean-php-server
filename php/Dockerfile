FROM arm64v8/php:8.0.21-fpm-alpine

RUN apk add wget git unzip zlib-dev libpng-dev libzip-dev libpq-dev icu-dev iputils autoconf gcc g++ make linux-headers unixodbc-dev gnupg openssh-keygen
RUN docker-php-ext-install bcmath zip gd intl sockets pcntl

WORKDIR /var/www

CMD ["php-fpm"]