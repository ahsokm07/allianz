FROM nginx:alpine
RUN chmod g+rwx /var/cache/nginx/ /var/run /var/log/nginx
RUN mkdir -p /var/www
COPY ./html /var/www/
COPY nginx.conf /etc/nginx/nginx.conf
EXPOSE 8000
