FROM alpine:latest
LABEL maintainer Felix Breidenstein <mail@fleaz.me>

RUN apk add --update tor
RUN apk update && \
    apk add tor  py3-pip --no-cache && \
    pip --no-cache-dir install nyx && \
    rm -rf /etc/apk/cache

# ORPort, DirPort, SocksPort
EXPOSE 9001 9030 9050 9051

VOLUME /var/lib/tor
VOLUME /etc/tor/torrc

CMD ["/usr/bin/tor"]
