#
# Dockerfile for dirsearch
#

FROM python:3.13.0a1-alpine
MAINTAINER EasyPi Software Foundation

RUN pip3 install --no-cache-dir pip install https://github.com/maurosoria/dirsearch/archive/refs/heads/master.zip

ENTRYPOINT ["dirsearch"]
CMD ["--help"]
