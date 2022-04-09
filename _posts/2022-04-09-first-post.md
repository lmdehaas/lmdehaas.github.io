---
layout: post
title:  "First (test) post"
date:   2022-04-09 16:23:37 +0200
categories: personal
---
{% highlight python %}
def binary_search(array, target):
    low = 0
    high = len(array) - 1
    while low <= high:
        mid = (low + high) // 2
        guess = array[mid]
        if guess == target:
            return mid
        if guess > target:
            high = mid - 1
        else:
            low = mid + 1
    return None
{% endhighlight %}