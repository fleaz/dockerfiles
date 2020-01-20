FROM ubuntu:xenial
LABEL maintainer Felix Breidenstein <mail@fleaz.me>

RUN apt-get update &&\
    apt-get install -y \
        awscli \
		jq \
        python3-pip \
        zip &&\
    rm -rf /var/lib/apt/lists
