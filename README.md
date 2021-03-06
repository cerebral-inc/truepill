# Truepill API Client

A ruby gem for the Truepill API.

Truepill API documentation: https://docs.truepill.com/#introduction

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'truepill'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install truepill

## Usage

First configure the environment and credentials.

In a Rails app, this might go in `config/initializers/truepill.rb` for example.

```ruby
Truepill.configure do |config|
  config.environment = Rails.env.production? ? :production : :sandbox
  config.api_key = ENV['TRUEPILL_API_KEY']
end
```

## Contributing

Bug reports and pull requests are welcome on GitHub at: [https://github.com/cerebral-inc/truepill](https://github.com/cerebral-inc/truepill)

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
