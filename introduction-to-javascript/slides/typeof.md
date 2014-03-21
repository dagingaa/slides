##  typeof

````javascript
// Numbers
typeof 37 === 'number';
typeof 3.14 === 'number';
typeof Infinity === 'number';
typeof NaN === 'number'; // Despite being "Not-A-Number"

// Strings
typeof "" === 'string';
typeof "bla" === 'string';

// Booleans
typeof true === 'boolean';
typeof false === 'boolean';

// Undefined
typeof undefined === 'undefined';
typeof blabla === 'undefined'; // an undefined variable

// Objects
typeof {a:1} === 'object';
typeof [1, 2, 4] === 'object';
typeof new Date() === 'object';

// Functions
typeof function(){} === 'function';
````

note:
    Put your speaker notes here.
    You can see them pressing 's'.
