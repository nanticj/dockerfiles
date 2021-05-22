FROM nanticj/debian:stable-20210511-slim

RUN curl -sSL https://get.haskellstack.org/ | sh && \
  stack setup && \
  echo 'eval "$(stack --bash-completion-script stack)"' >> ~/.bash_profile && \
  stack --version && \
  echo "2.7.1"

CMD bash
