source 'http://rubygems.org'

ruby '2.1.2'

# Load this project as a gem.
gemspec
gem "mysql2"

gem 'yard', :groups=>[:development, :test]
gem 'bluecloth', :groups=>[:development, :test] # For YARD
# gem 'query_reviewer' # Enable for performance tuning

gem "thin" # To avoid annoying Ruby 1.9.3/Rails/Webrick warnings - See http://stackoverflow.com/questions/7082364/what-does-warn-could-not-determine-content-length-of-response-body-mean-and-h

# Uncomment to confirm that older versions work (for compaitiblity with Spree 2.2.4/bcms_spree)
# gem 'paperclip', '~> 3.4.1'
# For testing behavior in production
group :production do
  gem 'uglifier'
end

group :development do
  gem 'rake'
  gem 'byebug'
  gem 'quiet_assets'
end
group :test, :development do
  gem 'minitest'
  gem 'minitest-rails'
  gem 'minitest-reporters'
end

group :test do
  gem 'rspec-expectations', '2.14.1'
  gem 'poltergeist'
  gem 'm', '~> 1.2'

  gem 'single_test'
  gem 'factory_girl_rails', '3.3.0'
  gem "mocha", '0.14.0', :require=>false
  gem "sqlite3-ruby", :require => "sqlite3"

  # Cucumber and dependencies
  gem 'capybara'
  gem 'database_cleaner'
  gem 'cucumber-rails', :require=> false
  gem 'cucumber'
  gem 'launchy'
  gem 'ruby-prof'
  gem 'aruba', '0.5.3'
end
