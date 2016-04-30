source "https://rubygems.org/"

gemspec

group :development do
  gem "jruby-openssl", :platform => :jruby
  gem "rcov", ">= 0.9.8", :platform => :mri_18
  gem "childprocess", :platform => :mri
  gem "maven-tools", "~> 0.34.5"
end

group :development, :test do
  gem 'rdoc', '~> 2.4.2', :require => nil
  gem 'rake', ENV['RAKE_VERSION'], :require => nil if ENV['RAKE_VERSION']
end

if ENV['RUBYZIP_VERSION']
  gem 'rubyzip', ENV['RUBYZIP_VERSION']
elsif RUBY_VERSION < "1.9"
  gem 'rubyzip', '~> 0.9'
end