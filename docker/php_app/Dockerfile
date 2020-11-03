FROM php:7.4-fpm-alpine
 
RUN apk update --no-cache \
&& apk add \
icu-dev \
oniguruma-dev \
tzdata

WORKDIR /php_app/

RUN docker-php-ext-install intl

RUN docker-php-ext-install pcntl

RUN docker-php-ext-install mbstring
 
RUN rm -rf /var/cache/apk/*
 
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer

RUN apk add --no-cache git

CMD ["php-fpm"]