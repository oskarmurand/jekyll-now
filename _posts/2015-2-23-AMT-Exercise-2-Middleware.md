---
layout: post
title: WebDev2 AMT Exercise 2 - Interactions with Middleware using ACS database
tags: [amt, android, ios, titanium, alloy, middleware, acs]
categories: [AMT]
---

# Exercise 2 description
> Create another window or view displaying a list (use tableView) of products of your own choice from Verifone webshop.

> Add login functionality by using data from cloud services (middleware).

---

# AMT: Exercise 2 Solution #

During the second day of AMT class we explored creating windows inside of the phone application (just like hyperlinks) and middleware usage for connecting to a database on the server.

## Windows ##
For learning how to use windows in Titanium Studio we used a small [exercise video]( https://www.youtube.com/watch?v=CB26lUj0UBQ) on youtube made by [Appcelerator]( http://www.appcelerator.com/).

Getting the links working and redirecting the user based on positive or negative result to a query was fairly straight forward if followed instructions.

![Win2 close, windows example](https://dl.dropboxusercontent.com/u/259275/blog/images/win2%20screenshot%20with%20window%20close%20label.png)

## Middleware ##

[Appcelerator Cloud Services](http://docs.appcelerator.com/cloud/latest/#!/guide/acs_quickstart) (*ACS*) by Appcelerator provides a set of REST APIs that we will be using for our data management.

The idea was to create a cloud service that we could use for login. This will be required for later exercises. Our solution will be tested by using [Postman](https://chrome.google.com/webstore/detail/postman-rest-client/fdmmgilgnpjigdojojpjoooidkmcomcm) Chrome Extention. (*I still need to find something nice for Firefox that achieves the same functionality.*)

Ofcourse doing this, at basically every step it is essential to read the [documentation](http://docs.appcelerator.com/titanium/latest/). Thanks Appcelerator!

In order to use Appcelerator Cloud Solution one will need to create an Appcelerator account and create a database on their server for free trough the [My Apps](https://my.appcelerator.com/apps) menu.

![appcelerator database image](https://dl.dropboxusercontent.com/u/259275/blog/images/Screen%20Shot%202015-02-23%20at%2010.09.35.png)



---
