# Twitter typeahead.js jquery plugin

This asset gem packages the [twitter typeahead.js](https://github.com/twitter/typeahead.js) jquery plugin for the Rails asset pipeline.

To learn more about typeahead.js read the post [Twitter's engineering blog](http://engineering.twitter.com/2013/02/twitter-typeaheadjs-you-autocomplete-me.html).

This gem includes the standard and minified versions of the assets.

## Installation

Add this line to your application's Gemfile:

    gem 'twitter-typeahead-rails'

    or

    gem 'twitter-typeahead-rails', :git => "git://github.com/yourabi/twitter-typeahead-rails.git"
    

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install twitter-typeahead-rails

## Usage

To start using the twitter typeahead.js plugin in your rails app enable it via the asset pipeline (app/assets/javascripts/application.js).

Add one the folllwing to your application.js mainifest:

```js

//= require twitter/typeahead                                                                                                                                                                                                                             

//= require twitter/typeahead.min                                                                                                                                                                                                                        

```


```js

// Twitter typeahead exmaple.
$(document).ready(function() {
  $('.typeahead').typeahead( {name: 'planets', local: [ "Mercury", "Venus", "Earth", "Mars", "Jupiter", "Saturn", "Uranus", "Neptune" ] });
});

```

You'll also probably want to enable include the CSS in your application.css manifest. Include one of the following:

```js

*= require twitter/typeahead

*= require twitter/typeahead.min

```

Currently this version tracks version v0.8.0.

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
