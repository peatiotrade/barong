[travis]: https://travis-ci.org/peatiotrade/barong
[www.peatio.trade]: https://www.peatio.trade

# Barong
[![Build Status](https://travis-ci.org/peatiotrade/barong.svg?branch=master)][travis]


# Overview

Barong is oAuth server for [peatio.trade][peatio.tech] stack.

# Development

Prerequisites:
- Ruby version: `2.5.1`
- Bundler preinstalled
- MySQL preinstalled

1. Install RubyGems dependencies
```
bundle install
```

2. Copy initialisation files
```
bin/init_config
```

3. Create database and run migrations
```
bundle exec rake db:create db:migrate
```

4. Install JS dependencies
```
yarn install
```

5. Start local server
```
bundle exec rails server
```

# Test client application

You can find example of Barong usage here: [Barong Test Client App](https://github.com/rubykube/barong-client-app)

[How to get client app credentials](./docs/oauthclient.md)

# Barong Levels

In the process of verification Barong assign different levels to accounts

- Level 0 is default account level
- Level 1 will apply after email verification
- Level 2 will apply after phone verification
- Level 3 will apply after identity & document verification

# License
Barong is released under the terms of the [Apache License 2.0](./LICENSE.md).
