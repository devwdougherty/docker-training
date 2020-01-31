FROM frolvlad/alpine-gcc

RUN apk add --no-cache g++
RUN apk add --no-cache cmake
RUN apk add --no-cache rapidjson-dev
RUN apk add --no-cache make
RUN apk add --no-cache curl
RUN apk add --no-cache nano

COPY . /usr/src/myapp
COPY ./myscript.sh /usr/src/scripts/myscript.sh

WORKDIR /usr/src/myapp

RUN /usr/src/scripts/myscript.sh
RUN g++ -o myapp test.cpp

EXPOSE 9081

