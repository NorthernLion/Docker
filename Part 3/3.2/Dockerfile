FROM ubuntu:16.04


RUN apt-get update && \
    apt-get install -y wget ffmpeg python3-pip python3-crypto python3-requests python3-lxml php-cli php-bcmath php-xml php-curl && \
    pip3 install --user --upgrade yle-dl

WORKDIR /areena

CMD ["/bin/bash"]

