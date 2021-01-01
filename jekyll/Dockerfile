FROM nanticj/bundler:2.7.2

EXPOSE 4000
WORKDIR /home

COPY ./Gemfile ./
RUN bundle install

CMD bundle exec jekyll serve --host 0.0.0.0
