# Ruby Installation Guide

## Required Software

- **Ruby**: Install from [ruby-lang.org](https://www.ruby-lang.org/en/downloads/) or using a version manager:
  - **rbenv**: [github.com/rbenv/rbenv](https://github.com/rbenv/rbenv)
  - **RVM**: [rvm.io](https://rvm.io/)
- **Bundler**: Gem management (`gem install bundler`)

## File Extensions

- `.rb` - Ruby source files
- `.erb` - Embedded Ruby template files
- `.gem` - Ruby gem package
- `.rake` - Rake task files
- `.gemspec` - Gem specification files
- `.ru` - Rack configuration files

## Package Management

```bash
# Create a new gem
bundle gem my_gem

# Install dependencies from Gemfile
bundle install

# Update dependencies
bundle update

# Execute a command in bundled environment
bundle exec command

# Install a gem
gem install gem_name
```

## Running Ruby Programs

```bash
# Run a Ruby script
ruby script.rb

# Run with warnings
ruby -w script.rb

# Check syntax without running
ruby -c script.rb

# Run with debug
ruby -d script.rb

# Interactive Ruby console
irb
```

## Common Libraries

- **Web Frameworks**: Ruby on Rails, Sinatra, Hanami
- **Testing**: RSpec, Minitest, Cucumber
- **HTTP**: Faraday, Rest-Client, HTTParty
- **Background Jobs**: Sidekiq, Resque, Delayed Job
- **ORM**: ActiveRecord, Sequel
