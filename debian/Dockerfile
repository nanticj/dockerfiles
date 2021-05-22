FROM debian:stable-20210511-slim

ENV USER=root
SHELL ["bash", "-lc"]

RUN apt update && apt install -y \
  bash-completion \
  bzip2 \
  curl \
  g++ \
  gcc \
  git \
  gnupg \
  libbz2-dev \
  libffi-dev \
  libgmp-dev \
  liblzma-dev \
  libreadline-dev \
  libsqlite3-dev \
  libssl-dev \
  make \
  netbase \
  xz-utils \
  zlib1g-dev \
  && rm -rf /var/lib/apt/lists/*

CMD bash
