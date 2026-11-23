# Shellwords

This module manipulates strings according to the word parsing rules
of the UNIX Bourne shell.

The `shellwords()` function was originally a port of shellwords.pl,
but modified to conform to [the Shell & Utilities volume of the IEEE
Std 1003.1-2008, 2016 Edition].

[the Shell & Utilities volume of the IEEE Std 1003.1-2008, 2016 Edition]: http://pubs.opengroup.org/onlinepubs/9699919799/utilities/contents.html

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'shellwords'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install shellwords

## Usage

```ruby
require 'shellwords'

argv = Shellwords.split('three blind "mice"')
argv #=> ["three", "blind", "mice"]
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake test` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`.

To release a new version, update `Shellwords::VERSION` in `lib/shellwords.rb`.
Push the release commit to `master` and wait for CI to pass. Then create and
push a matching `vX.Y.Z` tag on that commit. The [publish workflow] builds the
gem, publishes it to [RubyGems.org], and creates a GitHub release.

[publish workflow]: https://github.com/ruby/shellwords/actions/workflows/push_gem.yml
[RubyGems.org]: https://rubygems.org/gems/shellwords

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/ruby/shellwords.
