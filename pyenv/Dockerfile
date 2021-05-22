FROM nanticj/debian:stable-20210511-slim

RUN git clone https://github.com/pyenv/pyenv.git ~/.pyenv && \
  cd ~/.pyenv && \
  git checkout tags/1.2.27 && \
  echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile && \
  echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile && \
  echo 'eval "$(pyenv init -)"' >> ~/.bash_profile

CMD bash
