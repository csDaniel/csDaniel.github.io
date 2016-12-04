---
layout: post
title:  "Uploading my First Code Sample"
date:   2016-12-4 13:15:01 +0900
categories: story
---

Today I attempted to upload a simply python test set. Even during my time in university, I had difficulties running python with command line arguments on my local machine. To be honest, I usually just would complete most testing remote to the Linux server. 

{% highlight python %}
def helloBack():
	print("{}".format(sys.argv[0]))
	print("{}".format(sys.argv[1]))
{% endhighlight %}

Is a fairly simple implementation. However, this would always return that error:
{% highlight html %}
helloBack()IndexError: list index out of range
{% endhighlight %}
Rather than rack my brain on what I did 9 months ago regarding setting up root access for pyton, or what dependencies I’m missing, I’m just going to opt for a fresh install and go from there. In the end, I had to reset the path variable in order to properly execute [python from the command line](http://pythoncentral.io/add-python-to-path-python-is-not-recognized-as-an-internal-or-external-command/). Prior, I would just run the executable from the command line and that worked. Oh well. It’s all a learning process.
Next, I wanted to implement a fizzbuzz, because why not? The first dumb question I had was “how to check if it’s an integer?” This of course is not the correct question at all, which I realized the moment I ran the test, since the results would just truncate anyways. So, I checked if it were digits, then converted the argument to a long and it all worked out. Later, I went and modified the small program to allow for internal commands, such as running from a range of already defined ints. This required some minor overhead to perform a check to see if the input was a string or an int being passed into the fizzbuzz(). 
