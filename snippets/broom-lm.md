---
title: "Tidying linear models"
author: "David Robinson"
layout: snippet
category: broom
image: broom-lm/coef_plot-1.png
---

We perform a simple linear fit:


{% highlight r %}
fit <- lm(mpg ~ wt + qsec, mtcars)
{% endhighlight %}

Then `broom` makes it easy to create a coefficient plot with ggplot2:


{% highlight r %}
library(broom)
td <- tidy(fit, conf.int = TRUE)

library(ggplot2)
ggplot(td, aes(estimate, term, color = term)) +
    geom_point() +
    geom_errorbarh(aes(xmin = conf.low, xmax = conf.high)) +
    geom_vline()
{% endhighlight %}

![center](/broom-gallery/images/broom-lm/coef_plot-1.png) 
