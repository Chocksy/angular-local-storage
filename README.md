angular-local-storage
=====================

I'm going to add the option to store objects by using JSON.parse and JSON.stringify in this service.
==

An Angular module that gives you access to the browsers local storage

Remember to set your app name (settings.appPrefix) in the settings at the beginning of localStorageModule.js.

To do:
- Add tests
- Expand Readme

Example use: 

```javascript
angular.module('yourModule', ['LocalStorageModule'])
.controller('yourCtrl', [
  '$scope',
  'localStorageService',
  function($scope, localStorageService) {
    // Start fresh
    localStorageService.clearAll();
    localStorageService.add('Favorite Sport','Ultimate Frisbee');
}]);
```
Check out the full demo and documentation at http://gregpike.net/demos/angular-local-storage/demo.html
