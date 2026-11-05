#
# Dockerfile for tiddlywiki
#

FROM node:26.13.0-alpine3.24
MAINTAINER EasyPi Software Foundation

RUN npm install -g tiddlywiki

VOLUME /data
WORKDIR /data

EXPOSE 8080

ENTRYPOINT ["tiddlywiki", ".", "--listen", "host=0.0.0.0", "port=8080"]
