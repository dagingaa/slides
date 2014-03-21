##  Custom Objects - `new`

````javascript
function Person(first, last) {
    this.first = first;
    this.last = last;
    this.fullName = function() {
        return this.first + ' ' + this.last;
    };
    this.fullNameReversed = function() {
        return this.last + ', ' + this.first;
    };
}
var me = new Person("Dag-Inge", "Aas");
````

With `new` we can create constructor functions. Similar to Java.

note:
    Put your speaker notes here.
    You can see them pressing 's'.
