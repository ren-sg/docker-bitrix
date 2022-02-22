FROM nginx:latest

COPY ./nginx.conf /etc/nginx/
COPY ./upstream.conf /etc/nginx/conf.d/
COPY ./sites-available/ /etc/nginx/sites-available/

RUN usermod -u 1000 www-data

CMD ["nginx"]

EXPOSE 80 443
