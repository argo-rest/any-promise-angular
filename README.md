# AnyPromise adapter for AngularJS

[AnyPromise](https://github.com/argo-rest/any-promise) adapter for the
[AngularJS](https://angularjs.org/) framework.

## Usage

This adapter is implemented as an ES6 module which can be installed
with [jspm](https://jspm.io) and loaded via
[SystemJS](https://github.com/systemjs/systemjs) as follows:

``` javascript
import 'any-promise-http';

import angular from 'angular';

var mod = angular.module('example', ['anyPromise']);

mod.factory('exampleFactory', ['anyPromise', function(anyPromise) {
    // use anyPromise, e.g.
    return anyPromise.resolve(42);
}]);
```
