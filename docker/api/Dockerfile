FROM debian:stretch-slim

RUN  set -x \
    && apt-get update && apt-get install -y nginx wget python virtualenv vim curl python-pip python-twisted

COPY run.sh /run.sh
COPY helloworld.py /helloworld.py
COPY janus_url_generator.py /janus_url_generator.py

EXPOSE 8080

CMD  /run.sh
