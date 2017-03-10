FROM phusion/baseimage

#adding default variables
ARG NODE_ENV
ARG NODE_VERSION=latest

RUN echo "Install version: $NODE_VERSION"

RUN echo "Updating provisions"
RUN apt-get -q update
RUN apt-get install -y npm
RUN npm i -g n
RUN n $NODE_VERSION
RUN node -v

RUN echo "Defining ENV keys"
ENV NODE_ENV=$NODE_ENV
