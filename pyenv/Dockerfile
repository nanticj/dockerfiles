FROM debian:stable-slim

SHELL ["/bin/bash", "-lc"]

RUN apt update
RUN apt install -y bash-completion
RUN apt install -y build-essential
RUN apt install -y curl
RUN apt install -y git
RUN apt install -y libbz2-dev
RUN apt install -y libffi-dev
RUN apt install -y liblzma-dev
RUN apt install -y libreadline-dev
RUN apt install -y libsqlite3-dev
RUN apt install -y libssl-dev
RUN apt install -y zlib1g-dev

RUN git clone https://github.com/pyenv/pyenv.git ~/.pyenv
RUN echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile
RUN echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile
RUN echo 'eval "$(pyenv init -)"' >> ~/.bash_profile

CMD /bin/bash -l
