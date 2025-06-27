FROM nginx:latest

USER root

COPY index.html /usr/share/nginx/html/index.html
COPY nginx.conf /etc/nginx/nginx.conf

RUN mkdir -p /tmp/nginx/client_temp /tmp/nginx/proxy_temp && \
    chown -R nginx:nginx /tmp/nginx /usr/share/nginx/html

USER nginx
