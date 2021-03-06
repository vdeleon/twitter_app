Twitter App
===========
Twitter app to retrive tweets based on geo location and hash tag

* Author:  Prateek Mehrotra
* Contact: prateek123@gmail.com

Heroku
======
http://pm-twitter-app.herokuapp.com/

How it works:
======
https://github.com/prateekm21/twitter_app/wiki/Features

RSpec
=====
```
rake db:mongoid:create_indexes RAILS_ENV=test
bundle exec rspec -fd spec/models/* spec/controllers/* spec/integration/*
```

Run App locally
===============

```
rake db:mongoid:create_indexes
foreman start
```

  * For populating local DB with tweets
      * Go to `bundle exec rails c` under the app folder
      * `Resque.enqueue(Workers::Fetch::DownloadTweets)`


API Wiki
========
https://github.com/prateekm21/twitter_app/wiki
