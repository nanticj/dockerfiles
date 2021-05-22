FROM nanticj/debian:stable-20210511-slim

RUN curl -sSL https://repo.anaconda.com/miniconda/Miniconda3-py39_4.9.2-Linux-x86_64.sh -o miniconda.sh && \
  sh miniconda.sh -b && \
  ~/miniconda3/bin/conda init && \
  rm -rf miniconda.sh

CMD bash
