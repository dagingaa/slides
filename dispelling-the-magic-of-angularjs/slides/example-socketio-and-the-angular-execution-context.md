####  Example: socket.io and the Angular Execution Context

````javascript
var $scope.chatMessages = [];
socket.on("CHAT_MESSAGE", function (data) {
    $scope.chatMessages.push(data.message)
});
````

````html
<p ng-repeat="message in chatMessages">{{message}}</p>
````

<div class="fragment">
<pre><code class="javascript">var $scope.chatMessages = [];
socket.on("CHAT_MESSAGE", function (data) {
    $scope.$apply(function () {
        $scope.chatMessages.push(data.message)
    });
});
</code></pre>
</div>

note:
- Let's look at this example
- We get an event from the server, CHAT_MESSAGE
- Put the message into the $scope.chatMessages array
- What will happen to the view? (ask the audience)
- Nothing! Not until the next $digest cycle at least?
- Does anyone know what we have to do?
- We need to wrap everything inside the callback with $apply, so it enters the
  context
