FROM rust:1.68

#for alpine image (may not work)
#RUN apk update
#RUN apk --no-cache add openjdk17 --repository=https://dl-cdn.alpinelinux.org/alpine/v3.15/communit
#RUN apk add git


#for debian image
RUN apt-get update
RUN apt-get install openjdk-17-jdk -y

RUN rustup install nightly
RUN rustup target add x86_64-unknown-linux-musl
RUN rustup target add x86_64-unknown-linux-musl --toolchain nightly

WORKDIR /home/root
