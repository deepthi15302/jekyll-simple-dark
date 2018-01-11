---
layout: page
title: About
permalink: /about/
---

# simple-dark

A simple and dark theme for Jekyll. **Under development**

Responsive images, tables and iframes (for include videos of **Youtube**, **Vimeo** or similar services)
A minimal pure javascript code for toggle menu and responsive tables.
Icon font make with [Fontello](http://fontello.com/)

Support socials networks links (simple add the links on your _config.yml):

* Facebook
* Twitter
* Google+
* Pinterest
* Youtube
* Vimeo
* Instagram
* Linkedin

If you need a icon for others socials networks create a new issue on theme repository.

Browser compatibility:

* Firefox
* Chrome/Chromium
* Edge
* Internet Explorer 10
* Opera

## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "simple-dark"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: simple-dark
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install simple-dark

## Usage

### Social links:

For activate social links add these lines on your _config.yml:

```yaml
social_links: true  # If true show social links
facebook:
github:
gplus:
instagram:
linkedin:
pinterest:
twitter:
site.vimeo:
youtube:
```
Just add the ones you're going to use.

**Note:** gplus is for Google+ link.

### Responsive iframe for Youtube or Vimeo videos:

Insert the iframe code into a div whit the class **video** and remove **width** and **height** attributes, like this:

```html
<div class="video">
  <iframe  src="https://www.youtube.com/embed/<videoID>" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/son-link/jekyll-simple-dark
. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `simple-dark.gemspec` accordingly.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).