FROM ruby:2.5

RUN apt-get update -qq
RUN apt-get install -y nodejs postgresql-client
RUN gem install bundler

RUN mkdir /myapp
WORKDIR /app
COPY . /app
RUN bundle install

EXPOSE 3000
