FROM ubuntu:16.04

WORKDIR /mydir
COPY unicafe/ .
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN npm install
EXPOSE 3000
CMD npm start
