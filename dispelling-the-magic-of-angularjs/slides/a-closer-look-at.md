##  $apply

````javascript
function $apply(expr) {
  try {
    return $eval(expr);
  } catch (e) {
    $exceptionHandler(e);
  } finally {
    $root.$digest();
  }
}
````

note:
- So what does $apply do?
- $apply takes an expression (function) and executes it, handling exceptions as
  it goes.
- By doing this, all the work inside the expression is in the Angular Execution
  Context
- Subsequent calls to $apply will trigger an exception
- Once all the work is done, Angular will run $digest to notify watchers, which
  in turn will update the DOM of any changes made to $scope
