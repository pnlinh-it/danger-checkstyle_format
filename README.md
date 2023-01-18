[![Build Status](https://travis-ci.org/noboru-i/danger-checkstyle_format.svg?branch=master)](https://travis-ci.org/noboru-i/danger-checkstyle_format)

# danger-checkstyle_format

Danger plugin for checkstyle formatted xml file support `inline_mode`

## Installation

```
source "https://rubygems.pkg.github.com/pnlinh-it" do
  gem "danger-checkstyle_format", "0.1.1"
end
```

## Usage

<blockquote>Parse the XML file, and let the plugin do your reporting

```ruby
checkstyle_format.base_path = Dir.pwd
checkstyle_format.report('app/build/reports/checkstyle/checkstyle.xml', inline_mode = false)
```
</blockquote>

<blockquote>Parse the XML text, and let the plugin do your reporting

```ruby
checkstyle_format.base_path = Dir.pwd
checkstyle_format.report_by_text '<?xml ...'
```
</blockquote>

## Development

1. Clone this repo
2. Run `bundle install` to setup dependencies.
3. Run `bundle exec rake spec` to run the tests.
4. Use `bundle exec guard` to automatically have tests run as you make changes.
5. Make your changes.
