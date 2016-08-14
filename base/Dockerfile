FROM ubuntu:latest
MAINTAINER Reigner S. Yrastorza <reigner@yrastorza.us>

LABEL Description="My Docker Base Image" \
  buildDate="2016-08-12" \
  version="1.0"

ENV TERM=xterm-256color

WORKDIR /root

RUN apt-get update
RUN apt-get install -y python python-pip wget curl tar unzip iputils-ping vim openssl python-openssl ssl-cert 

CMD ["tail", "-f", "/var/log/messages"]
