FROM ubuntu:14.04
LABEL maintainer="jgi92@naver.com"

RUN apt-get update
RUN apt-get install -y nginx
RUN echo "\ndaemon off;" >> /etc/nginx/nginx.conf
RUN chown -R www-data:www-data /var/lib/nginx

VOLUME [ "/data", "/etc/nginx/site-enabled", "/var/log/nginx" ]

WORKDIR /etc/nginx

CMD ["nginx"]

EXPOSE 9000
EXPOSE 433