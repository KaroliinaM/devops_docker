FROM ubuntu:16.04

EXPOSE 5000

RUN apt-get update && apt-get install -y \
    curl && \
    curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs && \
    apt-get purge -y --auto-remove curl && \ 
    rm -rf /var/lib/apt/lists/*

WORKDIR /app
COPY frontend-example-docker-master .
RUN npm install

CMD npm start
