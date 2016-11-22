source ENV['GEM_SOURCE'] || "https://rubygems.org" 

group :development, :test do
  gem 'puppetlabs_spec_helper', :require => false
  gem "rspec", "< 3.2.0", { "platforms" => ["ruby_18"] }
  gem 'json_pure', '<= 2.0.1',  :require => false if RUBY_VERSION < '2.0.0'
  gem 'metadata-json-lint'
end

if puppetversion = ENV['PUPPET_GEM_VERSION']
  gem 'puppet', puppetversion, :require => false
else
  gem 'puppet', :require => false
end

# vim:ft=ruby
