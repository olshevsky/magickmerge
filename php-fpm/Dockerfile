FROM php:8.1-fpm-alpine
RUN apk update
RUN apk add imagemagick imagemagick-dev autoconf
RUN apk add --virtual build-dependencies build-base gcc wget git
RUN apk add --virtual build-dependencies build-base gcc
RUN pecl install imagick
COPY . /var/www
EXPOSE 9000
CMD ["php-fpm"]