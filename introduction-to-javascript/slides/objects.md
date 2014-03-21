###  Objects

<small>JavaScript objects can be thought of as simple collections of key-value pairs.</small>

````javascript
var obj = new Object();

// literal syntax, preferred!
var obj = {};

// Can be accessed in two ways. Dot notation cannot use reserved words.
obj.name = "Dag-Inge";
obj["name"];
> "Dag-Inge"

// Literal syntax can initialise objects
var obj = {
    name: "Dag-Inge",
    "humour": {
        fun: true
    }
};
````


note:
* JavaScript objects can be thought of as simple collections of name-value pairs.
* The "key" is a JavaScript string. The value can be any JavaScript value, including more objects.
