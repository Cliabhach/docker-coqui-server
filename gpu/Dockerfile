FROM tensorflow/tensorflow:2.9.1-gpu

RUN pip3 install --upgrade pip

COPY gpu/requirements.txt /tmp
RUN pip3 install --no-cache-dir -r /tmp/requirements.txt

ENTRYPOINT deepspeech-server --config /opt/deepspeech/config.json
