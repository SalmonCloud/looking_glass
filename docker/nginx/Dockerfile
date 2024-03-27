FROM nginx:mainline-alpine

COPY docker/nginx/nginx.conf /etc/nginx/nginx.conf
RUN rm -rf /usr/share/nginx/html/*
COPY *.js /usr/share/nginx/html/
