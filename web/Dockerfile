FROM php:5.6-apache

RUN docker-php-ext-install \
    mysql \
    mysqli

# Xdebug
RUN pecl install xdebug-2.5.5 && \
    docker-php-ext-enable xdebug
ADD ./php-xdebug.ini /usr/local/etc/php/conf.d/php-xdebug.ini

EXPOSE 80

CMD ["apache2-foreground"]
