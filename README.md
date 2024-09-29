# Rails project

## Devbox with rails
devbox init
devbox generate direnv
devbox add "ruby@3.3.4" "nodejs@20.17" "postgresql@15.7"
initdb

gem install rails
rails new . --skip-javascript --database=postgresql

gem install bundler
bundle install

## Config de la base de datos
Ponemos los campos de user password y database - lo mismo en el docker compose.

Por algo que no logro comprender al dejar el host como localhost ya le permite conectarse con la base de datos postgres local del docker

## Config de vite rails
gem 'vite_rails' to gemfile
bundle install
run: bundle exec vite install