FROM ubuntu:16.04

WORKDIR /mydir
RUN apt-get update && apt install -y curl git-core
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
EXPOSE 3000
CMD ["/bin/bash"]
