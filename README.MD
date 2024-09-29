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
gem 'vite_rails' to gemfile
run: bundle exec vite install