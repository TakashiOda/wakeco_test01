source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '2.7.1'

gem 'rails', '~> 6.0.3'
gem 'puma', '4.3.5'
gem 'sass-rails', '6.0.0'
gem 'webpacker', '5.1.0'
gem 'turbolinks', '5.2.1'
gem 'jbuilder', '2.10.0'
gem 'bcrypt', '3.1.13'
gem 'bootsnap', '1.4.6', require: false
gem 'font-awesome-rails', '4.7.0.5'
gem 'activeadmin','2.7.0'
gem 'devise','4.7.2'
gem 'omniauth'
gem 'omniauth-facebook','6.0.0'
gem 'omniauth-twitter','1.4.0'
gem 'omniauth-google-oauth2'
gem 'devise_token_auth'
gem 'rack-cors'
gem 'dotenv-rails'

group :development, :test do
  gem 'byebug',"11.1.3", platforms: [:mri, :mingw, :x64_mingw]
  gem 'sqlite3', '1.4.2'

end

group :test do
  gem 'rspec-rails', '~> 3.8'
  gem 'factory_bot_rails', '~> 5.1.0'
end

group :development do
  gem 'web-console', '4.0.4'
  gem 'listen', '3.2.1'
  gem 'spring', "2.1.0"
  gem 'spring-watcher-listen', '2.0.1'
  gem "pry", "0.13.1"
  gem 'pry-rails'
  gem 'foreman'
end
group :production do
  gem 'pg', '1.2.3'
end

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
