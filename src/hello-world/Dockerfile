FROM nginx:latest

USER root

COPY index.html /etc/nginx/html/index.html

RUN chown -R nginx:nginx /etc/nginx/ && \
    chown -R nginx:nginx /var/cache/nginx/

USER nginx
