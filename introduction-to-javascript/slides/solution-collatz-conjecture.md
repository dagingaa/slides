##  Solution: Collatz Conjecture

````javascript
var number = process.argv[2] || "1000";
var steps = 0;

while (number != 1) {
    if (number % 2 === 0) {
       number = Math.ceil(number / 2);
    } else {
        number = Math.ceil(number * 3) + 1;
    }
    steps++;
    console.log("Number is: " + number);
}

console.log("Steps taken: " + steps);
````

note:
    Put your speaker notes here.
    You can see them pressing 's'.
