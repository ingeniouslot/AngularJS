---
layout: post
title: "What is a module in AngularJS?"
description: ""
headline: ""
categories: "basic"
tags: [Architecture]
imagefeature:
comments: false
mathjax:
chart:
featured: false
---

A module is a block of code where you can collect and organize components like controllers, services, directives, and filters. It is a self contained block of code that can be pulled out of one application and dropped into another application.

## To create a new module

{% highlight javascript %}
angular
    .module('app', []);
{% endhighlight %}

**NOTE:** The second argument to the module is the list of dependencies for your module.

## To retrieve an exising module

{% highlight javascript %}
var app = angular
        .module('app');
{% endhighlight %}

this will return the existing **app** module.

