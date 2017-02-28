---
layout: post
title:  "Balanced typography with Tachyons CSS"
date:   2017-02-27 17:15:50 +0000
categories: technical 
---

Beautiful typography is something that software developers all too often overlook. Using themes such as Bootstrap, or creating websites straight from the PSDs of graphic designers causes us to miss out on understanding basic rules of style. 

I've always had a fondness for typography and as a front-end developer I've loved taking the work of the world-class graphic designers I've had the pleasure of working with throughout my career and turning them into working Apps. Recently, however I have started to explore what it is that makes beautiful type. This lead me to a wonderful book called [The Elements of Typographic Style](https://www.amazon.co.uk/Elements-Typographic-Style-Robert-Bringhurst/dp/0881792063) by Robert Bringhurst. 

As a web developer I am blessed with the ability to size fonts however I like. This wasn't a blessing that typographers of the past had. It was costly to create sizes so over time thought went into deciding what these sizes should be. Scales of fonts have similarites to musical scales - each font size should be a ratio of the one before it. Some of these type scales have been used for hundreds of years.

[Tachyons](http://tachyons.io) is an atomically designed CSS library and type scales are an important part of its design principles. In your HTML, you use one of 6 font sizes.

{% highlight html %}
<style>
.f1 { font-size: 3rem; }
.f2 { font-size: 2.25rem; }
.f3 { font-size: 1.5rem; }
.f4 { font-size: 1.25rem; }
.f5 { font-size: 1rem; }
.f6 { font-size: .875rem; }
</style>
<body>
  <h1 class="f1">Title</h1>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. </p>
</body>

{% endhighlight %}

There are font sizes specific to different window breakpoints to allow for responsive design. This can help to address the balance of sizing for different font sizes. In the code below, the h1 header will be at the font size 1.25rem in a small browser window size, in a medium browser window this will be 2.25rem and in a large browser window width it will be 3rem.

{% highlight html %}
<style>
</style>
<body>
  <h1 class="f4 f2-m f1-l">Title</h1>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. </p>
</body>

{% endhighlight %}

The Tachyons type scale is a useful starting point. With all my projects going forward, time will be spent developing a meaningful type scale.
