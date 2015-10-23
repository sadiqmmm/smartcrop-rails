# smartcrop-rails
[![Gem Version](https://badge.fury.io/rb/smartcrop-rails.svg)](http://badge.fury.io/rb/smartcrop-rails)

smartcrop-rails gem is the integration of smartcrop.js javascript library for your Rails 4 application.

Smartcrop.js implements an algorithm to find good crops for images.
Demo: For content aware image cropping http://29a.ch/2014/04/03/smartcrop-content-aware-image-cropping

source: https://github.com/jwagner/smartcrop.js/

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'smartcrop-rails'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install smartcrop-rails

Now you need to edit your `app/assets/javascripts/application.js` file and add the following line:
``` javascript
//= require smartcrop
```

## Usage

Here is the example working code to test with your Rails application.

Add this sample code to your `app/assets/javascripts/application.js` file

``` javascript
$(document).ready(function(){  
  
  SmartCrop.crop(image, {width: 100, height: 100}, function(result){console.log(result);});
	
});
```

*Note:* Here i am using `gem 'jquery-turbolinks'` for using the jquery $(document).ready function 


## Full documentation 

Read the smartcrop.js documentation here https://github.com/jwagner/smartcrop.js/

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake false` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/sadiqmmm/smartcrop-rails. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

