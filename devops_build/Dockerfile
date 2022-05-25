FROM nginx:1.17.3-alpine

LABEL MAINTAINER="marco"

ADD ./nginx.conf /etc/nginx/nginx.conf

RUN rm -rf /usr/share/nginx/html

ADD /build/ /usr/share/nginx/html