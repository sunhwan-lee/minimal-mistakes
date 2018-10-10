---
layout: posts
title:  "Create a personal academic website using Minimal Mistakes and Jekyll"
date:   2018-10-04
classes: wide
---

## Quick start and installation

In [Quick-Start Guide](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/), I chose a method to _Remove the Unnecessary_ method after forking [Minimal Mistakes repository](https://github.com/mmistakes/minimal-mistakes). 

The I updated `Gemfile` to host the site with GitHub Pages like this:
```
source "https://rubygems.org"

gem "github-pages", group: :jekyll_plugins

gem "minimal-mistakes-jekyll", :github => "mmistakes/minimal-mistakes"
gem "jekyll-remote-theme"

group :jekyll_plugins do
end
```
Also, after I added the following to `_config.yml` file,
```
remote_theme : "mmistakes/minimal-mistakes"
plugins:
  - jekyll-remote-theme
```
I ran `bundle update` to clear up any dependency issues, `bundle install`, and `bundle exec jekyll serve` to spin-up my site locally.

## Customization
### Change `_config.yml` file

* Changed skin to `contrast`
* Changed title
* Changed name
* Changed description
* Enabled search
* Modified Site Author

### Change `_data/navigation.yml` file

* Added Curriculum Vitae, Publication, and Blog to masterhead

-----

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
