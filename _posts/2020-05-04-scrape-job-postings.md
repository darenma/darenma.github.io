---
layout: post
title:  "A simple way to scrape the online job postings."
date:   2020-05-04 12:23:30 -0700
categories: jekyll update
---
As a new grad looking for jobs in Data Science, I always go to 
[Hacker News] for recently opened opportunities.
Despite of the old-school forum looking of the original thread, 
some people built this [simple but amazing mirror][hiring]
for "who's hiring" to help people read the job postings in bigger fonts and clear manner. 
Even better: you can search for keywords on the mirror.

Then I thought about making my own version for this mirror. Since I have to look 
for opportunities from various sources, it's better to have them dumped into one single location.
Here I will talk about how I applied what I learnt from Terence's class [Data Acquisition] to scrape the 
job lists and made my own searching engine in Jupyter Notebook.


{% highlight python %}
print("yes sir")
{% endhighlight %}



[Hacker News]: https://news.ycombinator.com/item?id=23042618
[hiring]: https://djqyo3vqv2.execute-api.us-west-1.amazonaws.com/latest/
[Data Acquisition]: https://github.com/parrt/msds692