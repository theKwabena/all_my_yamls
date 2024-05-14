FROM nginx:latest

VOLUME /etc/nginx/conf.d/
VOLUME /var/www/sites_available/:/etc/www/sites_available
VOLUME /var/log/nginx/:/var/log/nginx

RUN mkdir -p /certs

VOLUME ./certs/:/certs/

COPY ./certs/ /certs


COPY ./nginx.conf /etc/nginx/nginx.conf

EXPOSE 443
EXPOSE 80
EXPOSE 8080
