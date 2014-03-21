<h2 id="playing">Playing around with the DOM</h2>

<button id="clickMe" class="button" style="font-size: 20px">Click me!</button>

````html
<h2 id="playing">Playing around with the DOM</h2>
<button id="clickMe" class="button">Click me!</button>
````

````javascript
window.onload = function () {
    var button = document.getElementById("clickMe");
    button.addEventListener("click", function () {
        var header = document.getElementById("playing");
        header.innerHTML = "Hacking around with the DOM";
    });
};
````




note:
    Put your speaker notes here.
    You can see them pressing 's'.
