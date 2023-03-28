FROM rust:1.68

RUN apt-get update
RUN apt-get install openjdk-17-jdk -y

RUN rustup install nightly
RUN rustup target add x86_64-unknown-linux-musl
RUN rustup target add x86_64-unknown-linux-musl --toolchain nightly
