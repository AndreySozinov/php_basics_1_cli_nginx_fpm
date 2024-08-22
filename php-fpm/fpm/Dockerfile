FROM php:8.2-fpm

COPY ./php.ini /usr/local/etc/php/conf.d/php-custom.ini

RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli

WORKDIR /data

VOLUME /data

CMD ["php-fpm"]
