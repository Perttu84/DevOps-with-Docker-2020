FROM ruby:2.6.0
RUN apt-get update && apt-get install nodejs -y
RUN git clone https://github.com/docker-hy/rails-example-project.git
WORKDIR /rails-example-project
RUN bundle install && rails db:migrate
EXPOSE 3000
CMD rails s