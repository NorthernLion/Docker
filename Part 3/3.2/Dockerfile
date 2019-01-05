FROM ubuntu:16.04


RUN apt-get update && \
    apt-get install -y wget ffmpeg python3 python3-pip python3-setuptools python3-crypto python3-requests python3-lxml && \
    pip3 install yle-dl && \
    rm -rf /var/lib/apt/lists/* 

WORKDIR /app

ENV LC_ALL=C.UTF-8 

ENTRYPOINT ["yle-dl"]

