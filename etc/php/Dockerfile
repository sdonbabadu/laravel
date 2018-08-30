FROM php:7.2-fpm

# Replace shell with bash so we can source files
RUN rm /bin/sh && ln -s /bin/bash /bin/sh

RUN docker-php-ext-install mbstring \
        pdo_mysql \
        pdo

RUN useradd -u 1000 -ms /bin/bash app
USER app