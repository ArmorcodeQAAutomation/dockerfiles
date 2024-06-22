FROM	ruby:3.3.3-alpine3.20
LABEL maintainer "Jessie Frazelle <jess@linux.com>"

RUN apk add --no-cache \
	coreutils

RUN	set -x \
	&& apk add --no-cache --virtual .build-deps \
	build-base \
	&& gem install gmail-britta --no-document \
	&& apk del .build-deps
