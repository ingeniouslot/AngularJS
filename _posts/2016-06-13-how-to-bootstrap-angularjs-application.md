---
layout: post
mathjax: false
featured: false
comments: false
title: How to Bootstrap AngularJS Application
description: Describes different ways to initialize AngularJS Application
categories: "initialization"
headline: ''
modified: ''
tags: [Initialization]
imagefeature: ''
---
## Automatic Initialization

Place _**ng-app**_ to the root of your application, typically on the <html> tag if you want angular to auto-bootstrap your application.

{% highlight html %}
<!doctype html>
<html ng-app="moduleName">
  <body>
	...
    <script src="angular.js"></script>
  </body>
</html>
{% endhighlight %}

## Manual Initialization
If you need to have more control over the initialization process, you can use a manual bootstrapping method.

{% highlight html %}
<!doctype html>
<html>
  <body>
	...
    <div ng-controller="controllerName">
    ...
    </div>
    <script src="angular.js"></script>
  </body>
</html>
{% endhighlight %}

{% highlight javascript %}
angular.module('myApp', [])
.controller('controllerName', ['$scope', function ($scope) {
	...
}]);

angular.element(document).ready(function() {
	angular.bootstrap(document, ['myApp']);
});
{% endhighlight %}

**NOTE:** You should call angular.bootstrap() after you've loaded or defined your modules. You cannot add controllers, services, directives, etc after an application bootstraps.
