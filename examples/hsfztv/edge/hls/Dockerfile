FROM ossrs/srs:2.0

ADD hls.conf /etc/hls.conf

CMD \
    mkdir -p /data/root/live && \
    mkdir -p /data/log/hls && \
    objs/srs -c /etc/hls.conf

VOLUME ["/data"]
EXPOSE 1935

