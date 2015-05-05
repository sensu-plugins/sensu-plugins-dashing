## Sensu-Plugins-dashing

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-dashing.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-dashing)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-dashing.svg)](http://badge.fury.io/rb/sensu-plugins-dashing)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-dashing/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-dashing)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-dashing/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-dashing)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-dashing.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-dashing)
[ ![Codeship Status for sensu-plugins/sensu-plugins-dashing](https://codeship.com/projects/94441700-d5ad-0132-74aa-1e0a7d4d648e/status?branch=master)](https://codeship.com/projects/78141)

## Functionality

## Files
 * bin/handler-dashing.rb

## Usage

```
{
  "dashing": {
    "auth_token": "YOUR_AUTH_TOKEN",
    "host": "http://localhost:3030"
  }
}
```

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-dashing -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-dashing`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-dashing' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-dashing' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
