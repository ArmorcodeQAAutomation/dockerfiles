#
# Dockerfile for bittorrent-tracker
#

FROM node:20.14.0-alpine3.20
MAINTAINER EasyPi Software Foundation

RUN npm install -g bittorrent-tracker

EXPOSE 8000/tcp 8000/udp

ENTRYPOINT ["bittorrent-tracker"]
CMD ["--port", "8000"]
