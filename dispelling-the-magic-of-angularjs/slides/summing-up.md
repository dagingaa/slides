##  Summing up

````html
<div ng-app>
    <label>Name:</label>
    <input type="text" ng-model="yourName" placeholder="Enter a name here">
    <h1>Hello {{yourName}}!</h1>
</div>
````
1. Initiation -> Compilation -> Linking
4. native keydown event
5. Enter Angular Execution Context by using `$apply()`
6. Update $scope.yourName
6. $digest loop starts
7. $watch detects a change, notifies the interpolation directive
8. Update DOM
9. Exit Angular Execution Context
10. Browser re-renders the view

note:
- Angular finds the ng-app element and initiates itself
- Angular compiles the static template (DOMElement) within
- In the compilation phase, angular finds and sorts directives by priority
- Each directive's linking function is combined into a common linking function and returned
- A scope is created and passed into the linking function
- In the linking phase, the ng-model directive sets up listeners for the
  keydown event on the input element, and the interpolation directive watches
  the scope for changes using $watch
- A keydown event is fired, and ng-model is notified
- Enters the AEC by using $apply
- The scope is updated
- $digest is fired by $apply
- $watch detects a change and notifies the interpolation directive
- The interpolation directive updates the DOM
- $digest loop finishes when it detects no more dirty values
- The browser re-renders the view
