FROM ubuntu:xenial
LABEL maintainer Felix Breidenstein <mail@fleaz.me>

RUN apt-get update &&\
    apt-get install -y \
        jq \
        python3-pip \
        zip &&\
    rm -rf /var/lib/apt/lists

RUN pip3 install awscli
