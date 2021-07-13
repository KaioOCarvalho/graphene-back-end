FROM ubuntu:20.04

RUN apt-get update && apt-get upgrade -y && apt install apt-utils

RUN apt install python3-pip python3-dev -y

RUN pip3 install Flask

WORKDIR /test/graphql/src

EXPOSE 5000