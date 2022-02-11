FROM php:7.4.5-fpm

LABEL author="Khalid Sookia"

COPY php-fpm-pool.conf /etc/php/7.4.5/pool.d/www.conf

RUN echo 'date.timezone="Europe/Madrid"' >> /usr/local/etc/php/conf.d/date.ini

RUN groupadd dev -g 999
RUN useradd dev -g dev -d /home/dev -m

WORKDIR /var/www/dwwm

EXPOSE 9000
CMD ["php-fpm"]
