FROM localhost:5000/php56

RUN yum -y install httpd
RUN usermod -u 1000 apache
RUN groupmod -g 1000 apache

EXPOSE 80
EXPOSE 443

CMD ["/usr/sbin/httpd", "-DFOREGROUND"]
