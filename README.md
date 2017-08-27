## About

Hugo theme based on [Start Bootstrap Clean Blog](https://github.com/derrickshowers/hugo-clean-blog.git). Used as a starter, but may diverge to separate (unrelated) theme in the near future.

## Config

The following is an example of what can be added to *config.toml* for customization/features:

``` toml
baseurl = "http://humboldtux.github.io/sbcb-demo"
title = "Start Bootstrap Clean Blog"
canonifyurls = true
paginate = 10
theme = "startbootstrap-clean-blog"
languageCode = "en-us"
copyright = "Code released under the Apache 2.0 license."
googleAnalytics = "UA-123-45" # delete or comment to disable Google Analytics JS generation
disqusShortname = "YourDisqusShortname" #delete or comment to disable Disqus comments

[author]
  name = "Derrick Showers"

[params]
  DateForm = "Mon, Jan 2, 2006"
  Description = "Your site description"
  Author = "Derrick Showers"

  #Remove this line if you would prefer not to use an email button in the footer.
  email = "derrick@derrickshowers.com"

  # Number of post summaries to show on front page, comment out to allow default(4)
  postSummariesFrontPage = 4

  # Set to false to exclude read time from header of post
  showReadTime = true

  # Custom CSS and/or JS for overrides. Include in static directory.
  customCSS = ["css/foo.css"]
  customJS = ["js/foo.js"]

[[params.social]]
  title = "twitter"
  url = "https://twitter.com/humboldtux"
[[params.social]]
  title = "github"
  url = "https://github.com/humboldtux"
[[params.social]]
  title = "facebook"
  url = "https://www.facebook.com/FACEBOOKHANDLE"

[[menu.main]]
  name = "home"
  url = "/"
  weight = -200
[[menu.main]]
  name = "Archives"
  url = "/post/"
  weight = -180
```

The footer contains link icons to any enabled social media sites, such as Facebook and/or LinkedIn. There is also an email icon, by removing the `email` parameter.

## Customization

#### Custom CSS/JS

As you see in the example config above, custom CSS and JS files can be added using the `customCSS` and `customJS` keys. Once in your *config.toml*, make sure to also include the files in your static directory (at the exact path you chose in the config, so in a *css* or *js* directory based on the example).
