##  Connecting the model to the view

````javascript
// Registers a listener callback to be executed when the watchExpression changes
$watch(watchExpression, listener);

// Processes all the watchers of the current scope and all its children
$digest()

// Used to trigger a $digest from outside the angular framework
$apply(exp);

````

note:
- $watch
    - Register listeners that will fire when the watchExpression changes
    - Angular automatically registers all data bindings in the template as
      watchers of the scopes value
    - You can also register custom watchers, useful for doing stuff based on
      changes to a service
- $digest
    - Processes all watchers on the current scope and its children. Useful for
      testing mostly.
    - The $digest loop is run every time an event in the angular execution
      context is fired
    - The "magic" that, combined with watchers, sets up two-way databinding
    - Understanding if and when this fires is key to udnerstanding Angular
- $apply
    - Useful when you need to programatically trigger a $digest loop.
    - Not all events fire $digest. One example is socket.io
    - Must call $apply when manipulating the angular context to not break data
      binding
    - Avoid shotgunning $apply, understand it!
