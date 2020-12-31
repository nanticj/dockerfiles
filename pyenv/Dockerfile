FROM debian:stable-slim

SHELL ["bash", "-lc"]

RUN apt update && apt install -y \
  bash-completion \
  curl \
  g++ \
  gcc \
  git \
  libbz2-dev \
  libffi-dev \
  liblzma-dev \
  libreadline-dev \
  libsqlite3-dev \
  libssl-dev \
  make \
  zlib1g-dev \
  && rm -rf /var/lib/apt/lists/*

RUN git clone https://github.com/pyenv/pyenv.git ~/.pyenv && \
  echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile && \
  echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile && \
  echo 'eval "$(pyenv init -)"' >> ~/.bash_profile

CMD bash
