Katip
=========

This is a Change Logging gem for a git initialized project.

Katip is a gem which dumps the change log as a list grouped by version tags.
It also has an executable ruby file **daktilo**, which can be used in any git project.
Log rows will contain links to commits, commit note and contributer name.

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
  % daktilo
  Create CHANGELOG.md
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

and that's it. You have a CHANGELOG.md file on project root, generated based on your git commits and created release tags.

#### Links to resources

* Disqussion http://stackoverflow.com/questions/7387612/git-changelog-how-to-get-all-changes-up-to-a-specific-tag
* Example bash https://github.com/kandanapp/kandan/blob/master/gen-changelog.sh
* Example output https://github.com/kandanapp/kandan/blob/master/CHANGELOG.md
* https://github.com/pcreux/pimpmychangelog this repo add support github issue and authors

