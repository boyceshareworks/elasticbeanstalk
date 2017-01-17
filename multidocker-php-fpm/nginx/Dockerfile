FROM nginx

EXPOSE 80

RUN rm /etc/nginx/conf.d/default.conf
RUN apt-get update

WORKDIR /web/

RUN chown -R www-data:www-data /web

COPY ./nginx.conf /etc/nginx/


