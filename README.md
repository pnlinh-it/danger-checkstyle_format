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

## Debug with rubymine

```
Ruby script: /Users/pnlinh/.rvm/rubies/ruby-2.7.1/bin/bundle
Script arguments: exec danger local --dangerfile=/Users/pnlinh/Desktop/Dev/Android/android-boilerplate/Dangerfile.codecheck
Working directory: /Users/pnlinh/Desktop/Dev/Android/danger-checkstyle_format
Use other SDK: RVM:ruby-2.7.1
```
![image](https://user-images.githubusercontent.com/11713395/213198647-07e2334b-4b92-4d3e-a531-26e02311163b.png)

