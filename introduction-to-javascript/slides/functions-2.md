##  Functions contd.

````javascript
// Can take other functions as arguments
var filter = function(array, filterFunc) {
    var sum = 0;
    for (var i = 0; i < array.length; i++) {
        if (filterFunc(array[i])) {
            sum += array[i];
        }
    }
    return sum;
};

var bars = [1,2,3,4,5];
filter(bars, function (elem) {
    return elem % 2 !== 0;
});
````

note:
    Put your speaker notes here.
    You can see them pressing 's'.
