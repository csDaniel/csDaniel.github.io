---
layout: post
title:  "updates to site and projects"
date:   2016-12-8 20:48:01 +0900
categories: story
---

I’ve started altering the file chunks of this site. The next part for me is fixing the CSS and to make it more like something I’d like to see. To that end, [this is a nice breakdown of CSS with Jekyll]( http://markdotto.com/2014/02/28/including-css-in-jekyll/). 

However, I have to be honest? I really don’t like css. I find you’re either faced with two options when working with css: delicately maneuver through some monolithic style guide, like bootstrap or build your own style guide from scratch. From a developer’s perspective, the second option is probably the way to go. But I just find myself way too frustrated whenever I work with css. 

Instead, I just went back to the old method of [working with bootstrap]( http://getbootstrap.com/css/#overview). One of my goals for the night was just to make the nav-bar at the top of this site a dark color, and maybe change the background color to something not-white, and then set the content inside a white box. I guess the styling can stay for now and I’ll worry about that later?

Moving on, I’m working on a small project over at [this repo](https://github.com/csDaniel/pyJekyllPost). It’s takes my generic post, and adds the front matter to make it a proper .markdown post. The trickiest part I’m finding is modifying the [time to display]( https://docs.python.org/2/library/datetime.html) as the appropriate Jekyll format:
{% highlight html %}
Date:	YYYY-MM-DD HH:MM:SS +-TZ
{% endhighlight %}
