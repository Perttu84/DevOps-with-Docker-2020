FROM ubuntu

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install -y nodejs
RUN apt-get install git -y
RUN git clone https://github.com/docker-hy/frontend-example-docker.git
WORKDIR /frontend-example-docker
RUN npm install
EXPOSE 5000
CMD npm start