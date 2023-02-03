FROM riscv64/ubuntu:22.04

WORKDIR /root
RUN apt update && apt upgrade -yq && apt install wget libatomic1 -yq
RUN wget https://unofficial-builds.nodejs.org/download/release/v18.12.1/node-v18.12.1-linux-riscv64.tar.gz
RUN tar -xvf ./node-v18.12.1-linux-riscv64.tar.gz -C /opt
ENV PATH="${PATH}:/opt/node-v18.12.1-linux-riscv64/bin"
RUN node --version
RUN rm ./node-v18.12.1-linux-riscv64.tar.gz


