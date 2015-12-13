FROM localhost:5000/php56

RUN mkdir -p /var/www/laravel
WORKDIR /var/www/laravel

RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer

CMD ["bash"]
