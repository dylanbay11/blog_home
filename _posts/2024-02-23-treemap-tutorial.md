---
layout: post
title:  "Thinking 'Inside the Box' with Treemaps"
description: Picky about pie charts? Bored of bar charts? Try a treemap!
image: /assets/img/pretty-treemap.png
---


Everyone has seen a million bar charts, though they continue to be popular for a reason, and it's now popular wisdom that a pie chart should rarely be used simply because of, well, the stigma. Okay, that's unfair. The pie chart has some deeper problems. One of the fundamental issues has to do with how a pie chart uses its real estate. This isn't unique to pie charts, but space is limited for labels, and the whole center of the chart is essentially wasted space since the slivers are too hard to see (and no, a "donut chart" is not a real solution). Slice size is often unintuitive and hard to distinguish. For example, the following chart is very humorous and interesting, but as a chart itself, it's offensive to the eyes:

<figure>
	<img src="{{site.url}}/{{site.baseurl}}/assets/img/meta-piechart.png" alt=""> 
	<figcaption>It's meta, it's glorious, but still ugly. Source: ElephantEating on X (formerly Twitter)</figcaption>
</figure>

Well, there's good news. In almost every scenario in which you'd want to make a pie chart, you can make a treemap instead! And it will be much more socially acceptable. Not only that, but there are actually a number of other good scenarios where a treemap can be very useful, even cases where it might not be the first option that comes to mind. 

### How can I make a basic treemap? Is it really the same as a pie chart?

For our purposes, we'll be using the `treemap` package in R. 

{%- highlight r -%}
# Let's install and load the package
install.packages("treemap")
library("treemap")

# If you want to get started right away, you can generate an example dataset:
ex <- random.hierarchical.data(30)
# And then graph it. The short version: Index contains all category columns, vSize is the "actual data"
treemap(ex, index = names(ex)[1:(ncol(ex)-1)], vSize = "x")
{%- endhighlight -%}

One line graphing, ncie! Note that the core documentation has the complicated looking selection above for the columns. This is just so that the auto-generation works no matter how many columns you create. However, you can always just manually specify them as well and they will evaluate in order if you pass them as a vector of strings.

### Can I use the treemap for anything else?

You can, if you know your data well, do things "backwards" too, although of course a bar chart is always going to be a helpful and slightly more accurate option, if we're being honest. For example, in our grand rapids dataset COMPLETE ME

### So, when *exactly* should I use a treemap?

Basic treemap is a piechart replacer, or even a barchart, though this has drawbacks

a two or three layer deep barchart for heirarchical data and relationships, two is the sweet spot!

the highest level is pretty important, the others a bit less so, though you can play with this

NO NEGATIVES! Consider other solutions if this is the case. Ex: revenue reports, often colored red!

What's the visual benefit? The eye likes blocky things, it likes groups, size is a bit easier to judge than a pie chart, and you can see the "biggest" at a glance, if that's what you want to draw attention to.

Downsides/don't use: Weirdly sliced data, with either really boxy ones or really tiny ones, can look poor.

consider an interactive barchart for more complicated uses
example of this in the wild: windirstat or disk inventory 

<figure>
	<img src="{{site.url}}/{{site.baseurl}}/assets/img/diskinventoryx.png" alt=""> 
	<figcaption>In the app, you can click on bigger "folders" to zoom in and see what's inside! It's not the prettiest treemap I've ever seen, but it IS very effective in seeing everything "at a glance". Source: Wikipedia page</figcaption>
</figure>


