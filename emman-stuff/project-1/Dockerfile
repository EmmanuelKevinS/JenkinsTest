FROM ubuntu:22.04

RUN apt-get update && apt-get install -y g++

WORKDIR /myApp

COPY my-cpp-program.cpp /myApp

RUN g++ -o my-program my-cpp-program.cpp
