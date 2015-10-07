---
layout: post
title: Tags and Categories with Jekyll on Github Pages [Part 2]
tags: [jekyll, github]
categories: [jekyll]
---

This is an update to my [previous post]({% post_url 2015-2-10-Tags-And-Categories-With-Jekyll-On-Github-Pages %}) on using Tags and Categories with Jekyll on Github Pages. Obviously, my solution was not anything to brag about. Essentialy, the same functionality could be achieved by just listing some words in the bottom of every post. 

![face-palm](https://dl.dropboxusercontent.com/u/259275/blog/images/face-palm.gif)

So, I googled around and found an [elegant solution](http://codepen.io/oskarmurand/pen/VYyyKo) that actually works beautifully to give me categories. Awesome!

This code is pretty much all I need to insert to the default.html layout in order to generate the categories list in the Archive page. The other requirement is adding categories to posts. This I do in the header of the markdown files in YAML format - categories: [jekyll]

![high-five](https://dl.dropboxusercontent.com/u/259275/blog/images/high-five.gif)

***
Also, now we have [<i class="fa fa-flag"></i> Font Awesome](http://fortawesome.github.io/Font-Awesome/) for beautiful icons such as this:

[<i class="fa fa-twitter fa-5x"></i>](http://www.twitter.com/oskarmurand)
