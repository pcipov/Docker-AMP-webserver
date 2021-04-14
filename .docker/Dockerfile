FROM php:7.4-apache
RUN docker-php-ext-install mysqli
RUN a2enmod rewrite

ENV VERSION 1.0
LABEL version=$VERSION