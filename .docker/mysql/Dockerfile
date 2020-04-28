ARG PERCONA_VERSION

FROM percona:${PERCONA_VERSION}

LABEL maintainer="Osiozekhai Aliu"

CMD echo 10 > /proc/sys/vm/swappiness \
    && echo 1048576 > /proc/sys/fs/aio-max-nr