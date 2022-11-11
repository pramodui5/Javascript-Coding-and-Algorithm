# Javascript-Coding-and-Solutions
## Array methods
### 1. filter()
```
const ages = [32, 33, 16, 40];
const result = ages.filter(checkAdult);

function checkAdult(age) {
  return age >= 18;
}
console.log(result);
```
- The filter() method creates a new array filled with elements that pass a test provided by a function.
- The filter() method does not execute the function for empty elements.
- The filter() method does not change the original array.
