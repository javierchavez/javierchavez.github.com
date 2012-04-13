---
layout: base
title: My first post
published: true
excerpt: switching from wordpress
categories: blog
---

##{{ page.title }}

####Wordpress is for you if
*	your not a coder
*	you know you need a database
*	your not so good with the computer but you want a website.

####Jekyll is for you if
*	you are *or* wanabe a total geek
*	dont really see a need for a database
*	you really really want to learn something new.

####then you can make fun little automations for your site.
{% highlight ruby %}
namespace :jekyll do
  
  desc 'clean the _site folder'
  	task :clean do
  	system "rm -rf _site"
  end
  
end
{% endhighlight %}