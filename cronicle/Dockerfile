#
# Dockerfile for cronicle
#

FROM node:20.14.0-alpine3.20
MAINTAINER EasyPi Software Foundation

RUN set -xe \
    && apk add --no-cache bash coreutils curl jq procps tar \
    && curl -sSL https://raw.githubusercontent.com/jhuckaby/Cronicle/master/bin/install.js | node

WORKDIR /opt/cronicle
VOLUME /opt/cronicle/conf

ENV CRONICLE_foreground=1

EXPOSE 3012/tcp 3014/udp

ENTRYPOINT ["bin/control.sh"]
CMD ["start"]
