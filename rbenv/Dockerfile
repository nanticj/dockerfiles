FROM debian:stable-slim

SHELL ["/bin/bash", "-lc"]

RUN apt update
RUN apt install -y bash-completion
RUN apt install -y build-essential
RUN apt install -y curl
RUN apt install -y git
RUN apt install -y libssl-dev
RUN apt install -y zlib1g-dev

RUN git clone https://github.com/rbenv/rbenv.git ~/.rbenv
RUN git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
RUN cd ~/.rbenv && src/configure && make -C src
RUN echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
RUN echo 'eval "$(rbenv init -)"' >> ~/.bash_profile

CMD /bin/bash -l
