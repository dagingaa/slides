##  Variables and scope

* variables are declared with `var`

````javascript
var a = 1;
var b = "foo",
    c = "bar";
````

Blocks (such as `if`) do not have scope, only functions do.

````javascript
var foo = 1;
if (true) {
    var bar = foo;
    foo++;
}
bar;
````

<div class="fragment">
    <p>Variables are call by value, not call by reference!</p>
</div>

note:
    Put your speaker notes here.
    You can see them pressing 's'.
