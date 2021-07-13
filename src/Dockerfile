FROM ubuntu:20.04

WORKDIR /test/graphql/src

RUN apt-get update && apt-get upgrade -y && apt install apt-utils

RUN apt install python3-pip python3-dev -y

RUN apt install libpq-dev -y

COPY . /test/graphql/

RUN pip3 install -r requirements.txt

EXPOSE 5000

CMD ["python3", "flask_basic.py"]