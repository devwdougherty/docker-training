FROM frolvlad/alpine-gcc

RUN apk add --no-cache g++
#RUN apk add --no-cache cmake
#RUN apk add --no-cache rapidjson-dev

COPY ./API/ /usr/src/myapp
WORKDIR /usr/src/myapp
RUN g++ -o myapp test.cpp
CMD ["./myapp"]