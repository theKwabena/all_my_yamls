FROM nginx

VOLUME /etc/nginx/conf.d
VOLUME /var/www/sites_available
VOLUME /var/log/nginx


RUN mkdir -p /certs
COPY ./certs/ /certs


COPY ./nginx.conf /etc/nginx/nginx.conf

EXPOSE 443
EXPOSE 80
EXPOSE 8080
