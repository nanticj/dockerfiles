FROM nanticj/debian:stable-20210511-slim

RUN git clone https://github.com/rbenv/rbenv.git ~/.rbenv && \
  cd ~/.rbenv && \
  git checkout tags/v1.1.2 && \
  git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build && \
  cd ~/.rbenv && src/configure && make -C src && \
  echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile && \
  echo 'eval "$(rbenv init -)"' >> ~/.bash_profile

CMD bash
