FROM python:3-alpine

LABEL MAINTAINER mail@fleaz.me

RUN apk add gcc musl-dev && pip install mkdocs && apk del gcc musl-dev
