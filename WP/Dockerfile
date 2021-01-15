FROM php:7.4-apache


RUN apt update && apt install -y git 

WORKDIR /var/www/html

RUN git clone https://github.com/WordPress/WordPress.git .

RUN chown -R www-data:www-data /var/www/html

RUN docker-php-ext-install mysqli