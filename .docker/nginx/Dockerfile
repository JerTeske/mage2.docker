FROM pagespeed/nginx-pagespeed
LABEL maintainer="Osiozekhai Aliu"
RUN apk add --update netcat-openbsd bc curl wget git bash openssl tzdata curl libressl \
    && rm -rf /var/cache/apk/*;
COPY conf/nginx.conf /etc/nginx/nginx.conf
COPY conf/default.conf /etc/nginx/conf.d/default.conf
COPY conf/default_ssl.conf /etc/nginx/conf.d/default_ssl.conf
COPY docker-entrypoint.sh /usr/local/bin
RUN chmod +x /usr/local/bin/docker-entrypoint.sh