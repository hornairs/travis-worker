source :rubygems
gem 'resque',              '~> 1.17.0'
gem 'resque-meta',         '~> 1.0.3'
gem 'resque-heartbeat',    '~> 0.0.2'

platforms :mri_18 do
  gem 'SystemTimer'
end

gem 'vagrant',       "~> 0.7.8"

gem 'net-ssh'
gem 'net-ssh-shell'
gem 'hashr',         '~> 0.0.13'
gem "multi_json"

# amqp migration is a work in progress but it does not affect resque-based worker in any way
gem "amqp",         :git => "git://github.com/ruby-amqp/amqp.git"
gem "amq-client",   "~> 0.8.1"
gem "amq-protocol", "~> 0.8.0"
gem "eventmachine", ">= 1.0.beta3"

gem 'faraday', '~> 0.7.3'
gem 'rake', '~> 0.9.2'
gem 'thor'

platform :ruby do
  gem 'god'
end

group :development do
  gem 'yard', '~> 0.7.1'

  platform :ruby do
    gem 'rdiscount'
  end
end

group :debug do
  gem 'ruby-debug',   :platforms => :mri_18
  gem 'ruby-debug19', :platforms => :mri_19 unless RUBY_VERSION >= "1.9.3"
end

group :test do
  gem 'mocha'
  gem 'test_declarative'
  # gem 'web-socket-ruby'
  # gem 'fakeredis'
  # gem 'fakeweb'

  platforms :ruby_18 do
    gem 'minitest'
    gem 'minitest_tu_shim'
  end

  gem "evented-spec", :git => "git://github.com/ruby-amqp/evented-spec.git"
end
