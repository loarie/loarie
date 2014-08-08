---
layout: post
title: More Jekyll Fun
comments: true
---

Configuring scottloarie.com for my Githubpage was easier than I thought.

All I had to do was 

{% highlight js %}
$ echo "www.scottloarie.com" > CNAME
$ git add .
$ git commit -am "trying to configure scottloarie.com"
$ git push origin master
{% endhighlight %}

Going [here](https://github.com/loarie/loarie.github.io/settings) confirmed
>Your site is published at http://www.scottloarie.com.

Then I followed the the 'Access the Zone File' and 'Adding or Editing A Records' steps outlined [here](http://support.godaddy.com/help/article/680/managing-dns-for-your-domain-names)
to make sure the Zone Record 'Points to' 192.30.252.153 which I got [here](https://help.github.com/articles/tips-for-configuring-an-a-record-with-your-dns-provider)
While it said it might take some time to take effect, it worked immediately!