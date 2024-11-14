FROM tensorflow/tensorflow:2.2.3-py3
RUN pip install --no-cache-dir ludwig[full]
WORKDIR /data
ENTRYPOINT ["ludwig"]
