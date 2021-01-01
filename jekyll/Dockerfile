FROM nanticj/bundler:2.7.2

WORKDIR /home

COPY ./Gemfile ./
RUN bundle install

EXPOSE 4000
CMD bundle exec jekyll serve --host 0.0.0.0
