#
# Dockerfile for node-media-server
#

FROM node:20.15.1-alpine3.20
MAINTAINER EasyPi Software Foundation

WORKDIR /opt/nms

RUN npm install node-media-server

COPY app.js /opt/nms

EXPOSE 1935 8000

ENTRYPOINT ["sh", "-c"]
CMD ["node app.js"]
