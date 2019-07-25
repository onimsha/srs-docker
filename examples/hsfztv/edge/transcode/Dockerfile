FROM ossrs/srs:2.0-ffmpeg

ADD transcode.conf /etc/transcode.conf

CMD \
    mkdir -p /data/root/live && \
    mkdir -p /data/log/transcode && \
    objs/srs -c /etc/transcode.conf

VOLUME ["/data"]
EXPOSE 1935
