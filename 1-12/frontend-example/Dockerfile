FROM ubuntu
ENV API_URL=http://localhost:8000
RUN apt update && apt install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN git clone https://github.com/docker-hy/frontend-example-docker.git
WORKDIR /frontend-example-docker

EXPOSE 5000
RUN npm install
CMD npm start

