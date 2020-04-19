FROM ubuntu

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs
RUN apt-get install git -y
RUN git clone https://github.com/docker-hy/backend-example-docker
WORKDIR /backend-example-docker
RUN npm install
EXPOSE 8000
CMD npm start