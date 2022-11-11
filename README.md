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

### 2. find()
```
const ages = [3, 10, 18, 20];
const result = ages.find(checkAge);

function checkAge(age) {
  return age > 18;
}
console.log(result);
```
- The find() method returns the value of the first element that passes a test.
- The find() method executes a function for each array element.
- The find() method does not execute the function for empty elements.
- The find() method does not change the original array.

### 3. forEach()
```
const fruits = ["apple", "orange", "cherry"];
fruits.forEach(myFunction);

document.getElementById("demo").innerHTML = text;
 
function myFunction(item, index) {
  text += index + ": " + item + "<br>"; 
}
```
- The forEach() method calls a function for each element in an array.
- The forEach() method is not executed for empty elements.

### 4. includes()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
const result = fruits.includes("Mango");
console.log(result);
```
- The includes() method returns true if an array contains a specified value.
- The includes() method returns false if the value is not found.
- The includes() method is case sensitive.

### 5. indexOf()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let index = fruits.indexOf("Apple");
console.log(index);
```
- The indexOf() method returns the first index (position) of a specified value.
- The indexOf() method returns -1 if the value is not found.
- The indexOf() method starts at a specified index and searches from left to right.

### 6. map()
```
const numbers = [4, 9, 16, 25];
const newArr = numbers.map(Math.sqrt)
console.log(newArr);
```
- The indexOf() method returns the first index (position) of a specified value.
- The indexOf() method returns -1 if the value is not found.
- The indexOf() method starts at a specified index and searches from left to right.

### 7. reduce()
```
const numbers = [10, 2, 3, 5];
const result = numbers.reduce(getSum, 5);
function getSum(total, num) {
  return total + num;
}
console.log(result);
```
- The reduce() method executes a reducer function for array element.
- The reduce() method returns a single value: the function's accumulated result.

### 8. reverse()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon", "Pineapple");
console.log(reverseItem);
```
- The reverse() method reverses the order of the elements in an array.
- The reverse() method overwrites the original array.

### 9. push()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
const result = fruits.push("Kiwi", “Lemon”);

console.log(result);
```
- The push() method adds new items to the end of an array.
- The push() method changes the length of the array.
- The push() method returns the new length.

### 10. pop()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();
```
- The pop() method removes the last element of an array.
- The pop() method changes the original array.
- The pop() method returns the removed element.

### 11. shift()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();
```
- The shift() method removes the first item of an array.
- The shift() method changes the original array.
- The shift() method returns the shifted element.

### 12. slice()
```
const fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
const citrus = fruits.slice(1, 3);
console.log(citrus);
```
- The slice() method returns selected elements in an array, as a new array.
- The slice() method selects from a given start, up to a (not inclusive) given end.
- The slice() method does not change the original array.

### 13. sort()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();
console.log(fruits.sort());

Numeric Sort
const points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return a - b});
```
- The sort() sorts the elements of an array.
- The sort() overwrites the original array.
- The sort() sorts the elements as strings in alphabetical and ascending order.

### 14. splice()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
// At position 2, add 2 elements: 
fruits.splice(2, 0, "Lemon", "Kiwi");

const fruits = ["Banana", "Orange", "Apple", "Mango", "Kiwi"];
// At position 2, remove 2 items: 
fruits.splice(2, 2);
```
- The splice() method adds and/or removes array elements.
- The splice() method overwrites the original array.

### 15. toString()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let text = fruits.toString();
console.log(text);
Output: Banana,Orange,Apple,Mango
```
- The Array.toString() method returns a string with all array values 
    separated by commas:
- The toString() method does not change the original array.

### 16. unshift()
```
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon", "Pineapple");
console.log(fruits);
Output: Lemon,Pineapple,Banana,Orange,Apple,Mango
```
- The unshift() method adds new elements to the beginning of an array.
- The unshift() method overwrites the original array.

## javascript - Objects
### Possible ways to create objects in JavaScript
1. Object constructor:
	```
  var object = new Object();
  ```
2. Object's create method:
	```
  var object = Object.create(null);
  ```
3. Object literal syntax:
	```
  var object = { name: "Sudheer", age: 34 };
  ```
4. ES6 Class syntax:
	```
  class Person {
   		constructor(name) {  this.name = name; }
	}
	var object = new Person("Sudheer");
  ```
5. Singleton pattern:
	```
  var object = new function(){
   		this.name = "Sudheer";
	}
  ```
