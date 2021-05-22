FROM nanticj/debian:stable-20210511-slim

RUN echo "1.52.1" && \
  curl -sSL https://sh.rustup.rs -o rustup.sh && \
  sh rustup.sh -y && \
  rm -rf rustup.sh

CMD bash
