---
layout: post
title: Trying Jekyll
comments: true
---


<div class="message">
  Thought I'd kick off this blog with a quick justification for the technology choices I made...
</div>

Since recently moving from the [Carnegie Institution for Science](http://carnegiescience.edu/) to the [California Academy of Sciences](http://www.calacademy.org/) and loosing my [SUNet ID](https://accounts.stanford.edu/), I wanted to take the opportunity to rethink my personal website.

I wanted to keep things static (e.g. not [Rails](http://rubyonrails.org/)) and simple (e.g. not [Wordpress](http://wordpress.org/)) but wanted to include a blog, so I thought I'd check out [Githubs free hosting for Jekyll blogs](https://pages.github.com/).

Joshua Lande's [awesome blog post](http://joshualande.com/jekyll-github-pages-poole/) makes me think this will let me do pretty much everything I want and I figured it would be a nice chance to learn more about [Github pages](https://pages.github.com/), [Jekyll](http://jekyllrb.com/), [Poole](https://github.com/poole/poole), & [Markdown](https://en.wikipedia.org/wiki/Markdown).

So lets get started...

## What I did so far

>*fare thee well* [http://www.stanford.edu/~loarie](http://www.stanford.edu/~loarie)

1. Purchased [scottloarie.com](scottloarie.com) from [GoDaddy](http://www.godaddy.com/)
2. [Created a new repo](https://github.com/new) called [https://github.com/loarie/loarie.github.io](https://github.com/loarie/loarie.github.io)
3. Cloned poole into a new folder like so:
{% highlight js %}
$ mkdir personal_website
$ cd personal_website
$ git clone https://github.com/poole/poole.git .
$ git init
// made some minor changes
$ gem install jekyll
$ git commit -am "first commit"
$ git remote add origin https://github.com/loarie/loarie-loarie.github.io.git
$ git push -u origin master
{% endhighlight %}

Then I went to [http://loarie.github.io/](http://loarie.github.io/) and after waiting a bit, things seem to be rolling!

To make **this** post I just deleted the poole's example posts, and added a new one like so
{% highlight js %}
$ git rm _posts/*
$ cd _posts
$ mate 2014-08-08-trying-jekyll.md
// wrote this post
$ git add .
$ git commit -am "my first post"
$ git push -u origin master 
{% endhighlight %}

So far pretty cool and easy!

## Next steps

- Configure [scottloarie.com](scottloarie.com) for my Github page. I think [this](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages) will help with that
- Carry on with [Joshua Lande's post](http://joshualande.com/jekyll-github-pages-poole/) to learn how to customize things further
- Explore [Lanyon](https://github.com/poole/lanyon) with the help of [Patrick Steadman's post](http://patricksteadman.ca/2014/08/04/lanyonsetup/)
- Add some css to the site and add some more static pages

Stay tuned for more...
