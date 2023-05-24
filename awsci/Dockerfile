FROM ubuntu:jammy
LABEL maintainer Felix Breidenstein <mail@fleaz.me>

RUN apt-get update &&\
    apt-get install -y --no-install-recommends \
        ca-certificates \
        curl \
        file \
        jq \
        unzip \
        zip &&\
    rm -rf /var/lib/apt/lists

# Install json2env
RUN  cd /tmp &&\
    curl -L https://github.com/codemonauts/json2env/releases/download/v1.0.1/json2env_Linux_x86_64.tar.gz -o json2env.tar.gz &&\
    tar xvf json2env.tar.gz &&\
    mv json2env /usr/local/bin

# Install awscli2
RUN cd /tmp &&\
    curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" &&\
    unzip awscliv2.zip &&\
    ./aws/install
