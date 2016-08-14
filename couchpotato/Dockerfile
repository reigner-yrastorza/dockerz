FROM ryrastorza/x1:base
MAINTAINER Reigner S. Yrastorza <reigner@yrastorza.us>

LABEL Description="My Docker Base Image" \
  buildDate="2016-08-12" \
  version="1.0"

ENV TERM=xterm-256color \
  PYTHONIOENCODING="UTF-8"

WORKDIR /root
COPY [ "CouchPotatoServer.zip", "/root/" ]
RUN unzip /root/CouchPotatoServer.zip
RUN apt-get install -y git

EXPOSE 5050 5050

WORKDIR /root/CouchPotatoServer
CMD ["python", "CouchPotato.py"]
