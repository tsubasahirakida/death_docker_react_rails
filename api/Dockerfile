FROM ruby:2.7

ENV LANG=C.UTF-8 \
  TZ=Asia/Tokyo

WORKDIR /app
COPY Gemfile /app/Gemfile
COPY Gemfile.lock /app/Gemfile.lock
RUN bundle install

RUN apt-get update && apt-get install -y \
    nodejs \
    default-mysql-client

# Start the main process.
CMD ["rails", "server", "-b", "0.0.0.0"]
