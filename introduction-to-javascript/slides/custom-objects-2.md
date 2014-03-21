##  Custom Objects - `this`

````javascript
function newPerson(first, last) {
    return {
        first: first,
        last: last,
        fullName: function () {
            return this.first + " " + this.last;
        }
    };
}

var me = newPerson("Dag-Inge", "Aas");
me.fullName();
> "Dag-Inge Aas"

var fullName = me.fullName;
fullName();
> ?
````

<div class="fragment">
<p>Be careful with `this`!</p>
</div>


note:
When we call fullName(), 'this' is bound to the global object. Since there are no global variables called first or last we get undefined for each one.
