FROM ruby

RUN gem install rails

RUN apt update && apt install nodejs -y

ONBUILD RUN rails new myapp

ONBUILD WORKDIR myapp

ONBUILD RUN bundle install

#To run it:
#docker run -p 3000:3000 ID
