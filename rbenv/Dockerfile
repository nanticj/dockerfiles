FROM debian:stable-slim

SHELL ["bash", "-lc"]

RUN apt update && apt install -y \
  bash-completion \
  bzip2 \
  curl \
  gcc \
  git \
  libssl-dev \
  make \
  zlib1g-dev \
  && rm -rf /var/lib/apt/lists/*

RUN git clone https://github.com/rbenv/rbenv.git ~/.rbenv && \
  git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build && \
  cd ~/.rbenv && src/configure && make -C src && \
  echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile && \
  echo 'eval "$(rbenv init -)"' >> ~/.bash_profile

CMD bash
