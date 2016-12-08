---
layout: post
title:  "pyJekyllPost.py update 1"
date:   2016-12-8 21:48:01 +0900
categories: story
---

December 8, 2016
While working on the project, I found myself going back and forth to fix little problems that I should have caught early on. I realize it’s because **I didn’t design the app before I began working on it**. For example:

* How should a user run the file? 
* Where does the user data come from?
* How exactly should a user interact with the app?
Based on that thinking, I’ve taken a pause from writing out more of the app and instead sketching out how it should work. 

First, there should be a config file. This file should contain: layout types, a location of the /_posts/ folder, and a list of categories, built by the user. The user should be able to edit this config file from inside the app. 

Next, the execution of the app. For that, 
{% highlight python %}
>Python pyJekyllPost.py file.md “my new post”
select categories: a, b, c, d, …
> story, code
File created successfully at c:/website/_posts/my-new-post.markdown
{% endhighlight %}

But the user will need to set up some of the background stuff in that config file. 
{% highlight python %}
>python pyJekyllPost.py config <set>
Set output location:
>c:/website/_posts/
Clear categories? y/n
>y
Build categories list from posts? y/n
>y
Configuration set.
{% endhighlight %}

Near as I figure, available layouts, and categories can all be determined by knowing the file output location. Since Jekyll stores layouts in /_layouts/, there will either be default.html or there will be more. Handling custom layouts will be tricky. That next problem I guess is *does a custom post.html and page.html exist in a separate location?*
