FROM php:7.0-fpm

RUN apt-get update \
  && apt-get install -y zip unzip libzip-dev sqlite3 libsqlite3-dev libpq-dev libxslt-dev libmagickwand-dev libfreetype6-dev libjpeg62-turbo-dev libpng-dev \
  && pecl install imagick \
  && docker-php-ext-enable imagick \
  && docker-php-ext-install gd mbstring pdo_mysql pdo_pgsql pdo_sqlite xml zip
