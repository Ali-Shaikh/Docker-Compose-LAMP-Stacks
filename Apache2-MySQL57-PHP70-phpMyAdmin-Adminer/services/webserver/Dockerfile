FROM php:7.0.30-apache-jessie

MAINTAINER Ali Shaikh <ali.az.shaikh@gmail.com>
RUN apt-get -y update --fix-missing
RUN apt-get -y upgrade

# Other PHP7.0.30 Extensions

RUN apt-get -y install libmcrypt-dev
RUN docker-php-ext-install mcrypt

RUN apt-get -y install libsqlite3-dev libsqlite3-0 mysql-client
RUN apt-get -y install mysql-client
RUN docker-php-ext-install pdo_mysql 
RUN docker-php-ext-install pdo_sqlite
RUN docker-php-ext-install mysqli