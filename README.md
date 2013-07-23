# Katip

[![Gem Version](https://badge.fury.io/rb/katip.png)](http://badge.fury.io/rb/katip)
[![Code Climate](https://codeclimate.com/github/kebab-project/katip.png)](https://codeclimate.com/github/kebab-project/katip)
[![Dependency Status](https://gemnasium.com/kebab-project/katip.png)](https://gemnasium.com/kebab-project/katip)

This is a Change Logging gem for a git initialized project.

Katip is a gem which dumps the change log as a list grouped by version tags.
It also has an executable ruby file **katip**, which can be used in any git project.
Log rows will contain links to commits, commit note and contributor name.

## Installation

To install Katip just use:

```sh
gem install katip
```

When using bundler put it in your Gemfile:

```ruby
source 'https://rubygems.org'

gem 'katip'
```

## Usage

### Using the executable

In your git initialized project directory simply run

```sh
  % katip
  Create CHANGELOG.md
```

If you want to name your log file other than CHANGELOG.md

```sh
  % katip MyCustomFile.md
  Create MyCustomFile.md
```


### Using as a rake
Add gem in your Gemfile:

```ruby
source 'https://rubygems.org'

gem 'katip'
```

```sh
  % rake katip:create
  Create CHANGELOG.md
```

If you want to name your log file other than CHANGELOG.md

```sh
  % rake katip:create file=MyCustomFile.md
  Create MyCustomFile.md
```

and that's it. You have your change log file on project root, generated based on your git commits and created release tags.

#### Links to resources

* Disqussion http://stackoverflow.com/questions/7387612/git-changelog-how-to-get-all-changes-up-to-a-specific-tag
* Example bash https://github.com/kandanapp/kandan/blob/master/gen-changelog.sh
* Example output https://github.com/kandanapp/kandan/blob/master/CHANGELOG.md
* https://github.com/pcreux/pimpmychangelog this repo add support github issue and authors

## Bugs and  Feedback

If you discover any bugs or want to drop a line, feel free to create an issue on GitHub.

http://github.com/kebab-project/katip/issues

## Contributing

Cybele uses [TomDoc](http://tomdoc.org/), [rDoc](http://rubydoc.info/gems/cybele) and [SemVer](http://semver.org/), and takes it seriously.

Once you've made your great commits:

1. Fork Template
2. Create a topic branch - `git checkout -b my_branch`
3. Push to your branch - `git push origin my_branch`
4. Create a Pull Request from your branch
5. That's it!

## Credits

- Cybele is maintained and funded by [lab2023 - internet technologies](http://lab2023.com/)
- Thank you to all the [contributors!](https://github.com/kebab-project/katip/graphs/contributors)
- The names and logos for lab2023 are trademarks of lab2023, inc.

## License

Copyright 2012 lab2023 – internet technologies