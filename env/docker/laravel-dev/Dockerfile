FROM localhost:5000/php56

RUN mkdir /workspace
WORKDIR /workspace

RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer
RUN composer config -g repositories.packagist composer http://packagist.jp  # 高速化のため、有志が作ったミラーサーバーを使用

CMD ["bash"]
