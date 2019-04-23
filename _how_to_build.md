# Mac

Initial setup:
```
brew install ruby

PATH=/usr/local/opt/ruby/bin:$PATH
PATH=/usr/local/lib/ruby/gems/2.6.0/bin:$PATH

gem install bundler

bundle install
```

Run server:
```
bundle exec jekyll serve
```

# Additional Notes:

## Verify pages render correctly on phone

You can run the server on your computer and then verify the pages render correctly on a phone.  By default the server will only bind to local host, so it is not accessible on your local network.  Add `--host 0.0.0.0` to the `bundle exec` command to have the server bind to the external IP addresses on your computer.

## View future posts

Posts with future dates will not normally render.  Add `--future` to the `bundle exec` command to see these.
