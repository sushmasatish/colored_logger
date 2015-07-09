# ColoredLogger

Colored Logger provides a handy way to colorize your logs based on the log severity: (debug, info, warn, error, fatal, unknown, perf)

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'colored_logger'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install colored_logger

## Usage

```ruby
ColoredLogger::CLogger.debug("method_or_task_name","message to be logged")
ColoredLogger::CLogger.info("method_or_task_name","message to be logged")
ColoredLogger::CLogger.warn("method_or_task_name","message to be logged")
ColoredLogger::CLogger.error("method_or_task_name","message to be logged")
ColoredLogger::CLogger.fatal("method_or_task_name","message to be logged")
ColoredLogger::CLogger.unknown("method_or_task_name","message to be logged")
start_time = Time.now.ago(10.minute)
ColoredLogger::CLogger.log_time("method_or_task_name",start_time,"to finish job")
```

![alt tag](https://github.com/sushmasatish/colored_logger/blob/master/docs/demo_output.png)

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake rspec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/sushmasatish/colored_logger.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

