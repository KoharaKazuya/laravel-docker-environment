FROM localhost:5000/php56-apache

# working directory for setup
ADD laravel /var/www/laravel/
WORKDIR /var/www/laravel

# setup Apache
RUN echo 'DocumentRoot /var/www/laravel/public' >> /etc/httpd/conf/httpd.conf

# setup Laravel
RUN curl -sS https://getcomposer.org/installer | php
RUN php composer.phar install --prefer-dist
RUN chown -R apache:apache .
