FROM debian:jessie

EXPOSE 9000

RUN apt-get update
RUN apt-get install -y php5-fpm php5-mysql php5-mcrypt php5-gd php5-memcached php5-curl php5-xdebug php5-cli php5-intl php5-apcu 

RUN sed -i 's|listen = /var/run/php5-fpm.sock|listen = 0.0.0.0:9000|g' /etc/php5/fpm/pool.d/www.conf
COPY ./log.conf /etc/php5/fpm/pool.d/zz-log.conf

WORKDIR /web

RUN chown -R www-data:www-data /web

CMD /usr/sbin/php5-fpm -F
