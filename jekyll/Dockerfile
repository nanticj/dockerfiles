FROM nanticj/bundler:2.7.2

WORKDIR /home

COPY Gemfile Gemfile.lock ./
RUN bundle install

EXPOSE 4000
CMD bash
