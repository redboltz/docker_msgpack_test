FROM debian

MAINTAINER TAKATOSHI KONDO redboltz@gmail.com

RUN apt-get update
RUN apt-get install -y gcc
RUN apt-get install -y g++
RUN apt-get install -y clang
RUN apt-get install -y autoconf
RUN apt-get install -y automake
RUN apt-get install -y libtool

RUN apt-get install -y git
RUN apt-get install -y wget
RUN apt-get install -y unzip

RUN apt-get install -y make
RUN apt-get install -y cmake

RUN apt-get install -y zlib1g-dev
RUN apt-get install -y valgrind

RUN wget https://googletest.googlecode.com/files/gtest-1.7.0.zip
RUN unzip gtest-1.7.0.zip
RUN cd gtest-1.7.0 && cmake . && make
RUN cp -r /gtest-1.7.0/include/gtest /usr/local/include
RUN cp /gtest-1.7.0/*.a /usr/local/lib
