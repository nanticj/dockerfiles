FROM debian:stable-slim

SHELL ["bash", "-lc"]

RUN apt update && apt install -y \
  bash-completion \
  curl \
  gcc \
  git \
  && rm -rf /var/lib/apt/lists/*

RUN curl -sSL https://sh.rustup.rs -o rustup.sh && \
  sh rustup.sh -y && \
  rm -rf rustup.sh

ENV USER=root
CMD bash
