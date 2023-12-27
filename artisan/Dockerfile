FROM php:8.3-fpm-alpine

WORKDIR /var/www/html/steko_id

RUN docker-php-ext-install pdo_mysql

ENTRYPOINT ["php", "artisan"]