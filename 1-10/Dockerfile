FROM ubuntu

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs

# This requires the dockerfile to be in the same folder as the project's source code
COPY . /app
WORKDIR /app
RUN npm install
EXPOSE 5000
CMD npm start

