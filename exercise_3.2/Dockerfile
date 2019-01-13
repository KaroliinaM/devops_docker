FROM ubuntu:16.04

RUN apt-get update && apt-get install -y rtmpdump wget ffmpeg python3-dev python3-setuptools \
    python3-pip python3-crypto python3-requests python3-lxml \
    php-cli php-curl php-xml php-bcmath ffmpeg && \
    export LC_ALL=C.UTF-8 && \
    pip3 install --user --upgrade yle-dl && \
    echo export PATH=/root/.local/bin:$PATH >> ~/.bashrc && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /app

ENTRYPOINT ["/root/.local/bin/yle-dl"]
