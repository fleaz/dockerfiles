FROM ubuntu:bionic
LABEL MAINTAINER mail@fleaz.me
ENV LC_ALL=C.UTF-8
ENV LANG=C.UTF-8

RUN apt-get update &&\
    apt-get install --no-install-recommends -y python3-pip python3-setuptools &&\
    pip3 install wheel &&\
    pip3 install platformio

