---
layout: post
title: "Controllers in AngularJS"
description: ""
headline: ""
categories: "basic"
tags: []
imagefeature:
comments: false
mathjax:
chart:
featured: false
---

A controller is defined by a JavaScript constructor function. Controllers are used to control the data of angular applications. They contains attributes/properties and functions.

## To create a controller
{% highlight javascript %}
(function(){
    // creating a module
    angular.module('app', []);

    // controller function
    function MainController() {

    }

    angular
        .module('app')
        .controller('MainController', MainController);
})();
{% endhighlight %}

## Attach controller to DOM

Controller is attached to the DOM via the ng-controller directive.

{% highlight HTML %}

<div ng-controller="MainController">
  ...
</div>

{% endhighlight %}

When a controller is attached to the DOM Angular will instantiate a new Controller object, using the specified Controller's constructor function.



