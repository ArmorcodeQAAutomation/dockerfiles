#
# Dockerfile for obs-web-arm
#

FROM alpine:3 AS build
WORKDIR /app
RUN set -xe \
 && apk add --no-cache curl node npm tar \
 && curl -sSL https://github.com/Niek/obs-web/archive/refs/heads/master.tar.gz | tar xz --strip 1 \
 && npm install \
 && npm run build

FROM nginx:1.31.8-alpine3.24
MAINTAINER EasyPi Software Foundation
COPY --from build /app/public/* /usr/share/nginx/html
