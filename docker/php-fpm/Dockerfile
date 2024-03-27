FROM php:8.1-fpm-bullseye

RUN apt-get update && \
    apt-get --no-install-recommends -y install iputils-ping mtr traceroute iproute2 && \
    rm -rf /var/lib/apt/lists/*

COPY --chown=www-data:www-data . /usr/share/nginx/html/
COPY --chown=www-data:www-data docker/php-fpm/src/config.php /usr/share/nginx/html/config.php

