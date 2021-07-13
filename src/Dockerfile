FROM ubuntu:20.04

RUN apt-get update && apt-get upgrade -y && apt install apt-utils

RUN apt install tzdata -y

ENV TZ Asia/Colombo

RUN apt install postgresql postgresql-contrib -y

RUN apt install python3-pip python3-dev -y

RUN apt install libpq-dev -y

RUN pip3 install Flask \
    Flask-GraphQL \
    Flask-GraphQL-Auth \
    SQLAlchemy \
    graphene \
    graphene-sqlalchemy \
    psycopg2

WORKDIR /test/graphql/src

EXPOSE 5000/tcp