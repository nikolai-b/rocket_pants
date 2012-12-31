source :rubygems

# Allow testing multiple versions with Travis.
rails_version = ENV['RAILS_VERSION']
if rails_version && rails_version.length > 0
  puts "Testing Rails Version = #{rails_version}"
  # Override the specific versions
  gem 'railties',     rails_version
  gem 'actionpack',   rails_version
  gem 'activerecord', rails_version
end

if (moneta_version = ENV["MONETA_VERSION"])
  gem 'moneta', moneta_version
end

# 2.10 for the moment changes some exceptions.
gem 'rspec', '~> 2.9.0'

if (wp_version = ENV['WILL_PAGINATE_VERSION'])
  gem 'will_paginate', wp_version
end

gemspec