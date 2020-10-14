source 'https://rubygems.org'

# Install omnibus
gem 'omnibus', '~> 7.0'

# Use Chef's software definitions. It is recommended that you write your own
# software definitions, but you can clone/fork Chef's to get you started.
# gem 'omnibus-software', github: 'chef/omnibus-software'
gem 'omnibus-software', git: '/home/bob/dev/omnibus-software', branch: 'curl-without-libidn2'

# This development group is installed by default when you run `bundle install`,
# but if you are using Omnibus in a CI-based infrastructure, you do not need
# the Test Kitchen-based build lab. You can skip these unnecessary dependencies
# by running `bundle install --without development` to speed up build times.
group :development do
  # Use Berkshelf for resolving cookbook dependencies
  gem 'berkshelf'

  # Use Test Kitchen with Vagrant for converging the build environment
  gem 'test-kitchen'
  gem 'kitchen-vagrant'
end

