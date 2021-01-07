FROM debian:stable-slim

SHELL ["bash", "-lc"]

RUN apt update && apt install -y \
  bash-completion \
  curl \
  g++ \
  gcc \
  git \
  make \
  && rm -rf /var/lib/apt/lists/*

RUN curl -sSLO https://github.com/Kitware/CMake/releases/download/v3.19.2/cmake-3.19.2-Linux-x86_64.tar.gz && \
  tar -C /usr/local -zxvf cmake-3.19.2-Linux-x86_64.tar.gz && \
  mv /usr/local/cmake-3.19.2-Linux-x86_64 /usr/local/cmake && \
  rm -rf cmake-3.19.2-Linux-x86_64.tar.gz && \
  echo 'export PATH="/usr/local/cmake/bin:$PATH"' >> ~/.bash_profile

CMD bash
