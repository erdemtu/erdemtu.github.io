---
layout: post
title:  "Tinkering with Jekyll #2: Cooking up a Rakefile"
date:   2015-08-17 13:51:40 +0300
categories:
---

I am working on automating some simple tasks like creating posts. After some googling, I ended up making a Rakefile with the help of [a blog post by Arjan van der Gaag](http://arjanvandergaag.nl/blog/creating-new-jekyll-posts.html) and [a github repo by Ellen Gummesson](https://github.com/gummesson/jekyll-rake-boilerplate).

I only handled the most common tasks which are creating a post, typing `bundle exec jekyll serve` and `bundle exec jekyll build`. For the time being I am not drafting any posts so I did away with that. Serve and build commands are really not that vital, but it is more convenient to just type `rake serve` and `rake build`.

[Here is a gist of it](https://gist.github.com/erdemtu/3b44d7f4b69c618b7a02). Note that I am using the `github-pages` gem to run Jekyll.

If you are looking for something more comprehensive, [Ellen Gummesson's Repo](https://github.com/gummesson/jekyll-rake-boilerplate) should fit the bill just fine. Since I am inexperienced with Rake and Ruby It was very helpful for writing my own Rakefile.

Oh, and I excluded the Rakefile since there is no need for it to be online with the rest of the site. I excluded the Gemfile for github-pages while I was at it. All I had to was add `exclude: ['Rakefile', 'Gemfile.lock', 'Gemfile']` to `_config.yml`. Never hurts to be tidy.
