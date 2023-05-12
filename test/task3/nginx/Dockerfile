FROM nginx
COPY nginx.conf /etc/nginx/nginx.conf
COPY index.html /data/www/index.html
VOLUME /usr/share/nginx/html
VOLUME /etc/nginx
VOLUME /var/log/nginx/log
EXPOSE 80
STOPSIGNAL SIGQUIT
CMD ["nginx-debug", "-g", "daemon off;"]
