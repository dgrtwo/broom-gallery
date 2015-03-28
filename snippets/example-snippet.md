---
title: "An Example Snippet"
author: "Your Name"
layout: snippet
image: example-snippet/unnamed-chunk-2-1.png
---

Here's one snippet to get you started.

* To edit this snippet, open `_R/example-snippet.Rmd` (or add new snippets in that folder!).
* To rebuild it, use the [rgallery](https://github.com/dgrtwo/rgallery) package, with the `build_gallery()` function.
* To view the page, go to the command line and do:

    jekyll serve --watch    

These snippets work just like any [knitr](http://yihui.name/knitr/) page. You can perform operations:


{% highlight r %}
summary(cars)
{% endhighlight %}



{% highlight text %}
##      speed           dist       
##  Min.   : 4.0   Min.   :  2.00  
##  1st Qu.:12.0   1st Qu.: 26.00  
##  Median :15.0   Median : 36.00  
##  Mean   :15.4   Mean   : 42.98  
##  3rd Qu.:19.0   3rd Qu.: 56.00  
##  Max.   :25.0   Max.   :120.00
{% endhighlight %}

And you can make a graph (which will pop up as a "teaser" on the main gallery page):

![center](/images/example-snippet/unnamed-chunk-2-1.png) 
