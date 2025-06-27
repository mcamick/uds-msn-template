FROM nginx:latest

USER root

COPY index.html /etc/nginx/html/index.html

RUN mkdir -p /var/cache/nginx/client_temp \
              /var/cache/nginx/proxy_temp \
              /var/cache/nginx/fastcgi_temp \
              /var/cache/nginx/uwsgi_temp \
              /var/cache/nginx/scgi_temp && \
    chown -R nginx:nginx /etc/nginx/ && \
    chown -R nginx:nginx /var/cache/nginx/ && \
    chmod -R 755 /var/cache/nginx/

USER nginx
