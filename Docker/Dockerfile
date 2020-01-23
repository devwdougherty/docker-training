FROM frolvlad/alpine-gcc

RUN apk add --no-cache g++

COPY ./API/ /usr/src/myapp

WORKDIR /usr/src/myapp

RUN g++ -o myapp test.cpp
