# jekyll-simple-dark

A simple and dark theme for Jekyll.

Responsive images, tables and iframes (for include videos of **Youtube**, **Vimeo** or similar services)
A minimal pure javascript code for toggle menu and responsive tables. Compatible with Google Analytics and jekyll-seo-tags.

Icon font make with [Fontello](http://fontello.com/)

Support socials networks links (simple add the links on your _config.yml):

* RSS
* Facebook
* Twitter
* Google+
* Pinterest
* Youtube
* Vimeo
* Instagram
* Linkedin
* Reedit
* Spotify
* Telegram
* GitLab
* GitHub
* Git

If you need a icon for others socials networks create a new issue on theme repository.

Browser compatibility:

* Firefox
* Chrome/Chromium
* Edge
* Internet Explorer 10
* Opera

## Installation

Add this lines to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-simple-dark"
gem "jekyll-paginator" # This line isn't necessary if you use github-pages
```

Add this lines to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-simple-dark
plugins:
- jekyll-paginate
paginate: 5 # Posts per page
paginate_path: "page:num/"
```

Rename **index.md** to **index.html** and change **layout** to *home*

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-simple-dark

### Social links:

For activate social links add these lines on your _config.yml:

```yaml
social_links: true  # If true show social links
rss: true # For add icon to link feed.xml
facebook:
git:
gitlab:
github:
gplus:
instagram:
linkedin:
reedit:
spotify:
pinterest:
telegram:
twitch:
twitter:
vimeo:
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

### Google Analytics:
For use Google Analytics include this line  on **_config.yml** and replace &lt;code> for your Google Analytics code:

```yaml
google-analytics: <code>
```
Where &lt;code> is your Google Analytics code.

### jekyll-seo-tag:
For use you only need add this plugin on the plugins array on **_config.yml**

### Icons:
This theme include somo icons ready to use.



## Contributing

Bug reports and pull requests are welcome on [GitHub](https://github.com/son-link/jekyll-simple-dark ) or [GitLab](https://gitlab.com/son-link/jekyll-simple-dark)
. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `simple-dark.gemspec` accordingly.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
