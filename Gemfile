# A sample Gemfile
source "https://rubygems.org"
ruby "2.0.0"

gem "rails", '~> 4.0.0'


gem 'sass-rails',   '~> 4.0.0'
gem 'coffee-rails', '~> 4.0.0'
gem 'less-rails'
gem 'uglifier', '>= 1.0.3'
# See https://github.com/sstephenson/execjs#readme for more supported runtimes
gem 'therubyracer', platforms: :ruby


gem 'jquery-rails'
gem 'select2-rails'
gem 'bootstrap-datepicker-rails'
gem 'rails-assets-listjs', '0.2.0.beta.4' # remember to maintain list.*.js plugins and template engines on update
gem 'i18n-js', git: 'git://github.com/fnando/i18n-js.git' # to avoid US-ASCII js.erb error
gem 'rails-i18n'

gem 'mysql2'
gem 'prawn'
gem 'haml-rails'
gem 'kaminari'
gem 'simple_form'
gem 'client_side_validations', git: 'git://github.com/bcardarella/client_side_validations.git', branch: '4-0-beta'
gem 'client_side_validations-simple_form', git: 'git://github.com/saveritemedical/client_side_validations-simple_form.git'
gem 'inherited_resources'
gem 'localize_input', git: "git://github.com/bennibu/localize_input.git"
gem 'daemons'
gem 'twitter-bootstrap-rails'
gem 'simple-navigation'
gem 'simple-navigation-bootstrap'
#gem 'meta_search', git: 'git://github.com/jetthoughts/meta_search.git' # other git repo for rails4; still breaks form_for -> ransack
gem 'acts_as_tree'
gem "rails-settings-cached", "0.3.1"
gem 'resque'
gem 'whenever', require: false # For defining cronjobs, see config/schedule.rb
gem 'protected_attributes'

# we use the git version of acts_as_versioned, and need to include it in this Gemfile
gem 'acts_as_versioned', git: 'git://github.com/technoweenie/acts_as_versioned.git'
gem 'foodsoft_wiki', path: 'lib/foodsoft_wiki'

group :production do
  gem 'exception_notification'
end

group :development do
  gem 'sqlite3'
  gem 'mailcatcher'
  
  # Better error output
  gem 'better_errors'
  gem 'binding_of_caller'
  # gem "rails-i18n-debug"
  
  # Get infos when not using proper eager loading
  gem 'bullet'

  # Hide assets requests in log
  gem 'quiet_assets'
  
  # Deploy with Capistrano
  gem 'capistrano', '2.13.5'
  gem 'capistrano-ext'
  #gem 'common_deploy', require: false, path: '../../common_deploy' # pending foodcoops/foodsoft#34,  git: 'git://github.com/fsmanuel/common_deploy.git'
  # Avoid having content-length warnings
  gem 'thin'
end

group :development, :test do
  gem 'ruby-prof'
end

group :test do
  gem 'rspec-rails'
  gem 'factory_girl_rails', '~> 4.0'
  gem 'faker'
  gem 'capybara'
  # webkit and poltergeist don't seem to work yet
  gem 'selenium-webdriver'
  gem 'database_cleaner'
  gem 'connection_pool'
  gem 'simplecov', require: false
  # need to include rspec components before i18n-spec or rake fails in test environment
  gem 'rspec-core'
  gem 'rspec-expectations'
  gem 'rspec-rerun'
  gem 'i18n-spec'
end
