FROM php:fpm-alpine

RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/bin/composer
RUN /usr/bin/composer self-update
RUN composer global require "laravel/lumen-installer"
RUN ln -s /root/.composer/vendor/bin/lumen /bin/lumen
