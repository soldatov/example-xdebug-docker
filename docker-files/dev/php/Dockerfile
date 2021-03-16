FROM php:8.0-fpm
# https://github.com/mlocati/docker-php-extension-installer
COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/local/bin/

RUN apt-get update && apt-get install \
    && install-php-extensions xdebug pdo_pgsql \
    && apt-get clean \
    && cp /usr/local/etc/php/php.ini-development /usr/local/etc/php/php.ini

COPY ./99-xdebug.ini /usr/local/etc/php/conf.d/99-xdebug.ini

WORKDIR /app
