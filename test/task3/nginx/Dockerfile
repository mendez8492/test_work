#FROM nginx
#RUN rm /etc/nginx/nginx.conf /etc/nginx/conf.d/default.conf
#COPY content /usr/share/nginx/html
#COPY conf /etc/nginx
#VOLUME /var/log/nginx/log
#EXPOSE 81
#STOPSIGNAL SIGQUIT
#CMD ["nginx-debug", "-g", "daemon off;"]

FROM nginx
COPY nginx.conf /etc/nginx/nginx.conf
COPY index.html /data/www/index.html
#COPY content /usr/share/nginx/html
#COPY conf /etc/nginx
VOLUME /usr/share/nginx/html
VOLUME /etc/nginx
VOLUME /var/log/nginx/log
EXPOSE 80
STOPSIGNAL SIGQUIT
CMD ["nginx-debug", "-g", "daemon off;"]
