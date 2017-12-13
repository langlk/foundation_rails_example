# README

## To Install Foundation

```
gem install foundation-rails
```

add ```gem "foundation-rails"``` to Gemfile
```
bundle update
rails g foundation:install
yarn add jquery
```

Your ```app/assets/javascripts/application.js``` requires should look like:
```JavaScript
//= require rails-ujs
//= require turbolinks
//= require jquery
//= require foundation
//= require_tree
```

Make a ```foundation_load.coffee``` file in ```app/assets/javascripts``` add add the following code:
```CoffeeScript
$(document).on('turbolinks:load', () ->
  $(document).foundation()
)
```
If you add any sass files that require foundation bits just add ```@import 'settings'``` at the top of the file.
