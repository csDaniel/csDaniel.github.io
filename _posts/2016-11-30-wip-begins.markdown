---
layout: post
title:  "wip begins"
date:   2016-11-30 20:02:01 +0900
categories: story
---


I began by following Eike’s advice with the github.io page. This has led to be following the guide at 
[pages.github.com](https://pages.github.com/). This set me up with a site hosted out of a simple domain. From there, I set about checking more information and came across [this youtube video](https://www.youtube.com/watch?v=nN6QuNqmAwk). This video is nearly 2 years old, so I wonder how out of date it is. 
[More installation instructions here](https://www.youtube.com/watch?v=iWowJBRMtpc). It is much better. After messing around, I ended up installing bundler. This allowed me to make a dumb template folder in my coding directory. Then I could simply copy + paste the content into the real sites folder. It now runs on local host. 

The next hurdle was changing the directory of the links. For starters, it’s represented as
 {% highlight html %}
 .../Jekyll/update/2016/11/29/post-title.html. 
 {% endhighlight %}
 
 I find that “Jekyll/update” to be a tad redundant. It stems from a student project in web development where I was working with the Yeoman scaffolding system and foolishly used my google drive for the git repo. This led to an insane depth of folder nesting. Don't be like me. Over on
[this blog](http://damonbauer.me/organizing-jekyll-pages/) there was some good information on how to fix that. It's fairly indepth and seems like a path I may one day take regarding organizing the posts on here. Another option is found in [the official documentation](http://jekyllrb.com/docs/home). In the front matter, change: 
{% highlight html %}
---
...
categories: jekyll update
---
{% endhighlight %}
to read 
{% highlight html %}
---
...
categories: blog
---
{% endhighlight %}
This elininates some of the depth of the folders. However, it still seperates posts into folders based on the day they were posted. To fix that, in the _config.yml, I needed to add at the bottom:
{% highlight html %}
permalink: none
{% endhighlight %}

I have continued the research on Jekyll. While the website lives, I don’t quite understand to details of it all just yet. Today I spent time reading over the official documentation to understand the file system and the hierarchy of the folders. For this I studied [the main website](https://jekyllrb.com/). I also took a look at the github repo for the default theme, [minima]( https://github.com/jekyll/minima). 

Next, I took a look at just [how to incorporate javascript into the pages for added effect](
http://blog.emmatosch.com/2016/03/09/using-custom-javascript-in-jekyll-blogs.html).

So now that I know how to do it, the next step is to just do it, right?