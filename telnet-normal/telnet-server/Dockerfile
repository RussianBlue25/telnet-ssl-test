FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install -y telnetd tcpdump
ARG TELNET_UID=1000
ARG TELNET_USER=docker
ARG TELNET_PASSWORD=docker
RUN useradd -ms /bin/bash ${TELNET_USER} \
  && echo ${TELNET_USER}:${TELNET_PASSWORD} | chpasswd

