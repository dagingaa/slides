##  Other operators

`&&`, `||`

<small>Uses short-circuit logic, and will execute their last operand dependent on the previous.</small>

````javascript
var name = obj && obj.getName();
name = name || "default";
````

`==` and `===`

<small>`==` does type coercion, `===` is strict equality</small>

````javascript
"1" == 1
> true

"1" === 1
> false
````

note:
    Put your speaker notes here.
    You can see them pressing 's'.
