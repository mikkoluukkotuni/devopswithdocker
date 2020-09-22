FROM ubuntu

# This tries to download project source code from GitHub during building
RUN apt update && apt install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN git clone https://github.com/docker-hy/backend-example-docker.git
WORKDIR /backend-example-docker

EXPOSE 8000
RUN npm install
CMD npm start

