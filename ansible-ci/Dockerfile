FROM jfloff/alpine-python:2.7-slim

MAINTAINER "Vladimir Iacob <vladimir.iacob@everymatrix.com>"

RUN apk add --no-cache sudo openssl ca-certificates
RUN apk add --no-cache --virtual build-dependencies libffi-dev openssl-dev build-base
RUN apk add --no-cache sshpass openssh-client rsync
RUN apk add --no-cache musl-dev linux-headers python-dev

RUN pip install ansible==2.4.2 shade==1.17.0 pywinrm==0.3.0 hvac==0.2.17

CMD [ "ansible-playbook", "--version" ]
