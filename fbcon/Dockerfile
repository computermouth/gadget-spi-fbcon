FROM arm32v7/debian:stretch-slim

RUN apt-get -y update &&\
 apt-get -y --no-install-recommends install cmatrix kmod &&\
 apt-get -y clean &&\
 rm -rf /var/lib/apt/lists/*

ENV HOME=/root

RUN echo "exec cmatrix" >> /root/.bashrc

ADD getty.sh /
