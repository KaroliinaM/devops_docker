FROM ubuntu:16.04

WORKDIR /mydir
COPY frontend-example-docker-master ./frontend
COPY backend-example-docker-master ./backend
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
EXPOSE 5000
EXPOSE 8000
RUN cd backend && npm install
RUN cd frontend && npm install
CMD ["/bin/bash"]
