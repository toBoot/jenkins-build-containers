FROM docker:23.0-cli

#ARG group=docker
#ARG gid=972

#RUN addgroup --gid ${gid} ${group}

RUN apk update
RUN apk --no-cache add openjdk17 --repository=https://dl-cdn.alpinelinux.org/alpine/v3.15/communit
RUN apk add git


WORKDIR /home/root
