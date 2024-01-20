FROM ubuntu:20.04

WORKDIR /usr/src/webapp

COPY webapp.sh .

RUN apt update
RUN apt install curl --yes

CMD ./webapp.sh