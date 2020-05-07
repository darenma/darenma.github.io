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

In order to get the raw text data of the thread, I decide to use Python's requests and BeautifulSoup packages.
These two are extremely useful together when we want to find the html content fulfilling certain rules.

{% highlight python %}
import requests
import pandas as pd
from bs4 import BeautifulSoup

url = "https://news.ycombinator.com/item?id=23042618"
r = requests.get(url)
{% endhighlight %}

TL;DR: You can view my [repo] here for the whole notebook.

[Hacker News]: https://news.ycombinator.com/item?id=23042618
[hiring]: https://djqyo3vqv2.execute-api.us-west-1.amazonaws.com/latest/
[Data Acquisition]: https://github.com/parrt/msds692
[repo]: https://github.com/darenma/data/blob/master/Hack%20Jobs/Job%20Postings%20on%20Hacker%20News.ipynb