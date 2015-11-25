FROM redis

MAINTAINER Abed Halawi <abed.halawi@vinelab.com>

COPY redis-primary.conf /etc/redis.conf

EXPOSE 6379
VOLUME /data

CMD ["redis-server", "/etc/redis.conf"]
