FROM ruby:2.7

ENV APPLICATION_ROOT /app/

RUN gem install sinatra json puma

WORKDIR $APPLICATION_ROOT
ADD . $APPLICATION_ROOT

EXPOSE 9292

ENTRYPOINT ["puma", "-e", "production"]
