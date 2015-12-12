FROM centos:6

# setup CentOS
RUN yum -y update

# setup PHP
RUN yum -y install epel-release  # 下記 remi が依存している
RUN rpm -Uvh http://rpms.famillecollet.com/enterprise/remi-release-6.rpm  # PHP 5.6 をインストールするため
RUN yum -y install --enablerepo=remi,remi-php56 php php-pdo php-mbstring php-xml  # Laravel の依存パッケージをインストール (php-xml は PHPUnit)

CMD ["php", "-r"]
