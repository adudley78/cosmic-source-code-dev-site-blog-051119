source 'https://rubygems.org'

gem 'bundler', '~> 2.0'
gem 'sinatra', '~> 2.0', '>= 2.0.4', require: 'sinatra/base'
gem 'eucalypt', '0.7.1'
gem 'rake', '~> 12.3'
gem 'thin', '~> 1.7'

# IRB is not bundled in Ruby >= 2.6
if Gem::Version.new(RUBY_VERSION) >= Gem::Version.new('2.6')
  gem 'irb', require: false
end

# Test environment
group :test do
  gem 'rack-test', '~> 1.0', require: 'rack/test'
  gem 'rspec', '~> 3.7'
  gem 'shoulda-matchers', '~> 3.1'
end

# Database adapters
gem 'sqlite3', '~> 1.3.6', group: [:development, :test]
gem 'pg', '~> 1.0', group: :production
# ActiveRecord for models and records
gem 'activerecord', '~> 5.2', require: ['active_support','active_support/core_ext']
gem 'sinatra-activerecord', '~> 2.0', require: ['sinatra/activerecord','sinatra/activerecord/rake']
# Logging library
gem 'lumberjack', '~> 1.0'
# Asset pipeline and preprocessors/compressors
gem 'sprockets', '~> 3.7'
gem 'sassc', '~> 1.12'
gem 'uglifier', '~> 4.1'
# Hanami HTML/asset helpers
gem 'hanami-helpers', '~> 1.2', require: 'hanami/helpers'
gem 'hanami-assets', '~> 1.2', require: ['hanami/assets','hanami/assets/helpers']