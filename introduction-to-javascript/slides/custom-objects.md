##  Custom Objects

````javascript
function newPerson(first, last) {
    return {
        first: first,
        last: last
    };
}

function fullName(person) {
    return person.first + " " + person.last;
}

var me = newPerson("Dag-Inge", "Aas");
fullName(me);
> "Dag-Inge Aas"
````

<div class="fragment">
<p>But this is kinda cumbersome, and not very readable either.</p>
</div>
note:
    Put your speaker notes here.
    You can see them pressing 's'.
