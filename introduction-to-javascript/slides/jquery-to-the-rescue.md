##  jQuery to the rescue

Because your time is too precious to deal with that shit.

* Common (cross-browser) API for DOM manipulation
* Slower, but delegates to internal APIs when possible
* DOM traversal using CSS-like selectors

````html
<h2 id="playing">Playing around with the DOM</h2>
<button id="clickMe" class="button">Click me!</button>
````

````javascript
$(function () {
    $("#clickMe").on("click", function () {
        $("#playing").html("Hacking around with the DOM");
    });
});
````



note:
    Put your speaker notes here.
    You can see them pressing 's'.
