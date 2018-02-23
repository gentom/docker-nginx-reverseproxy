FROM nginx
MAINTAINER gentom
#RUN rm /etc/nginx/conf.d/default.conf
COPY etc/nginx/conf.d/ /etc/nginx/conf.d/
#ENTRYPOINT /usr/sbin/nginx -g 'daemon off;' -c /etc/nginx/nginx.conf
CMD /usr/sbin/nginx -g 'daemon off;' -c /etc/nginx/nginx.conf