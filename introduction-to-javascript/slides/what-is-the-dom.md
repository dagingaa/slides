##  What is the DOM?

````html
<html>
    <head></head>
    <body>
        <ul id="list">
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </body>
</html>
````

````javascript
// returns an array
var html = document.getElementsByTagName("html");
var body = document.getElementsByTagName("body");
var li = document.getElementsByTagName("li");

// returns an object representation of the element
var ul = document.getElementById("list");
````


note:
* Document Object Model
* Programming interface for HTML and XML documents
* Defines a programmatic API to the structure of the document, so we can
  programatically cahnge it
