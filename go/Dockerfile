FROM nanticj/debian:stable-20210511-slim

RUN curl -LO https://golang.org/dl/go1.15.6.linux-amd64.tar.gz && \
  tar -C /usr/local -xzf go1.15.6.linux-amd64.tar.gz && \
  rm -rf go1.15.6.linux-amd64.tar.gz && \
  echo 'export PATH="/usr/local/go/bin:$PATH"' >> ~/.bash_profile

CMD bash
