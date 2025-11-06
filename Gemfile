source 'https://rubygems.org'

ruby '3.1.6'

gem 'rails',        '~> 6.1.7'
gem 'rails-i18n'
gem 'bcrypt'
gem 'faker'
gem 'bootstrap-sass'
gem 'will_paginate', '~> 3.3.1'
gem 'bootstrap-will_paginate', '~> 1.0.0'
gem 'puma',         '~> 5.0'
gem 'sass-rails',   '>= 6'
gem 'jquery-rails'
gem 'coffee-rails', '~> 5.0'
gem 'turbolinks',   '~> 5'
gem 'jbuilder',     '~> 2.7'

gem 'sqlite3', '~> 1.4'

group :development, :test do
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
end

group :development do
  gem 'web-console', '>= 4.1.0'
  gem 'listen', '~> 3.3'
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
  gem 'brakeman', require: false
  gem 'bundler-audit', require: false
end

# Windows環境ではtzinfo-dataというgemを含める必要があります
# Mac環境でもこのままでOKです
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]