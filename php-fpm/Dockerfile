ARG PHP_IMAGE_VERSION=fpm-alpine
FROM php:${PHP_IMAGE_VERSION}

RUN apk upgrade && \
    apk update && \
    apk add --update --no-cache \
      oniguruma-dev && \
    apk add \
      vim \
      git \
      composer && \
    docker-php-ext-install \
      pdo_mysql \
      mysqli \
      mbstring

WORKDIR /var/www/html
