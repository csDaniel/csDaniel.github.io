---
layout: post
title:  "Work Continues"
date:   2016-12-1 13:52:01 +0900
categories: story
---

Today I learned that if you change the root folder name of where you store any of your dependencies, it breaks everything and you need to re-install or reset all the permissions. Cool.
Otherwise I’m practicing with the different formatting that’s possible in [markdown]( https://en.support.wordpress.com/markdown-quick-reference/) as compared to html. It’s easier, for one. And by using 
{% highlight html %}
Jekyll serve –watch
{% endhighlight %}
I’m able to get informative error messages that tells me what I’m screwing up. So I spent time today going back and toying with [post #2]( https://csdaniel.github.io/blog/wip-begins.html). I also took it as an opportunity to clean up some of the extra tabs at the top which were just testing and working with Jekyll.

The next task today was setting up tabs at the top to return lists of specific entries: stories and projects. Turns out my problem here was just in understanding the class structure of Jekyll, or rather ruby. Wwhen you use include in any markdown post, it translates it into html automatically. The dates were ugly until I read [here regarding Jekyll date formatting]( http://alanwsmith.com/jekyll-liquid-date-formatting-examples). 

