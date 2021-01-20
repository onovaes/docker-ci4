FROM php:7.4-fpm-alpine

RUN apk update --no-cache \
&& apk add \
icu-dev \
oniguruma-dev \
tzdata

#RUN apk add --no-cache $PHPIZE_DEPS \
#    && pecl install xdebug-2.9.2 \
#    && docker-php-ext-enable xdebug 

WORKDIR /php_app/

# CI ESSENTIALS
RUN docker-php-ext-install intl pcntl mbstring

# Installing composer
RUN rm -rf /var/cache/apk/*
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer
RUN apk add --no-cache git

CMD ["php-fpm"]