#
# Use build context ../ !!!!
#

FROM nginx:1.15

WORKDIR /var/www/html/

COPY ./docker-web-nginx/vhost.conf /etc/nginx/conf.d/default.conf

RUN chown -R www-data:www-data /var/www/