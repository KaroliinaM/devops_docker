FROM ubuntu:16.04

WORKDIR /mydir
COPY curlscript.sh .
RUN apt-get update && apt-get install -y curl
CMD ./curlscript.sh
