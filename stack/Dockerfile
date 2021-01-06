FROM debian:stable-slim

SHELL ["bash", "-lc"]

RUN apt update && apt install -y \
  bash-completion \
  curl \
  gcc \
  git \
  gnupg \
  libffi-dev \
  libgmp-dev \
  make \
  netbase \
  xz-utils \
  zlib1g-dev \
  && rm -rf /var/lib/apt/lists/*

RUN curl -sSL https://get.haskellstack.org/ | sh && \
  stack setup && \
  echo 'eval "$(stack --bash-completion-script stack)"' >> ~/.bash_profile

CMD bash
