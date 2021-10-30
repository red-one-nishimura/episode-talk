FROM php:7.4-fpm

ADD ./docker/php/php.ini /usr/local/etc/php/php.ini

# composerをインストール
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

#mysql etc
RUN apt-get update && apt-get install -y git libzip-dev zip unzip bash gcc make libpng-dev vim
RUN docker-php-ext-install zip
RUN docker-php-ext-install pdo_mysql