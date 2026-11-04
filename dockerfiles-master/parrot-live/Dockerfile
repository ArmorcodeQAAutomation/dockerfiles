FROM node:26.13.0-alpine3.24

RUN apk add --no-cache git
RUN git clone --branch master --depth 1 https://github.com/hugomd/parrot.live.git /src
WORKDIR /src
RUN npm install
CMD ["node","index.js"]
