FROM alpine:edge

RUN apk update && apk add --no-cache vlc ffmpeg ffmpeg-libs jpeg libjpeg-turbo v4l-utils tzdata

RUN addgroup -g 1000 vlc && adduser -D -u 1000 -G vlc vlc
USER vlc

ENTRYPOINT ["/bin/sh","-c","cvlc"]