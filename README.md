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
### Math Object
``` Math.round(x) ```	Returns x rounded to its nearest integer

``` Math.ceil(x) ```	Returns x rounded up to its nearest integer

``` Math.floor(x) ```	Returns x rounded down to its nearest integer

``` Math.trunc(x) ```	Returns the integer part of x (new in ES6)

``` Math.round(4.6); ```

- The pop() method removes the last element of an array.
- The pop() method changes the original array.
- The pop() method returns the removed element.

### JSON and its operations
Parsing: Converting a string to a native object
	``` JSON.parse(text) ```

converting a native object to a string
	``` JSON.stringify(object) ```
	
### slice() Vs Splice()
#### Slice					
- Doesn't modify the original array(immutable)

- Returns the subset of original array

- Used to pick the elements from array	

#### Splice
- Doesn't modify the original array(immutable)

- Returns the subset of original array

- Used to pick the elements from array	

### Higher order function
Higher-order function is a function that accepts another function as an argument or returns a function as a return value or both.
```
const firstOrderFunc = () => console.log ('Hello, I am a First order function');
const higherOrder = ReturnFirstOrderFunc => ReturnFirstOrderFunc();
higherOrder(firstOrderFunc);
```
### Arrow Functions
Arrow functions allows a short syntax for writing function expressions.
You don't need the function keyword, the return keyword, and the curly brackets.
```
// ES5
var x = function(x, y) {
  return x * y;
}

// ES6
const x = (x, y) => x * y;
```
### Closures
A closure is the combination of a function and the lexical environment within which that function was declared. 
It is an inner function that has access to the outer or enclosing function’s variables. The closure has three scope chains

1. Own scope where variables defined between its curly brackets
2. Outer function’s variables
3. Global variables

#### Example - 1
```
function add(x) {
  return function(y) {
    return x + y;
  };
}

var add5 = add(5);
var add10 = add(10);

console.log(add5(2));  // 7
console.log(add10(2)); // 12
```
#### Example - 2
```
function displayName() {
  var name = 'Mozilla';
  function myName() {
    alert(name);
  }
  return myName;
}

var showName = displayName();
showName();
```
### Array.prototype.flat()
```
const arr1 = [0, 1, 2, [3, 4]];

console.log(arr1.flat());
// expected output: [0, 1, 2, 3, 4]

const arr2 = [0, 1, 2, [[[3, 4]]]];

console.log(arr2.flat(2));
// expected output: [0, 1, 2, [3, 4]]
```
- The flat() method creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.

### Generator Function
```
function* generator(i) {
  yield i;
  yield i + 10;
}
const gen = generator(10);
console.log(gen.next().value);
// expected output: 10
console.log(gen.next().value);
// expected output: 20
```
- The function* declaration (function keyword followed by an asterisk) defines a generator function, which returns a Generator object.

### call()
```
const person = {
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
}

const person1 = {
  firstName: "Mary",
  lastName: "Doe"
}

// This will return "Mary Doe":
person.fullName.apply(person1);
```
- The call() method calls a function with a given this value and arguments provided individually.
- The call() method takes arguments separately.
- The apply() method takes arguments as an array.

### apply()
```
const numbers = [5, 6, 2, 3, 7];
const max = Math.max.apply(null, numbers);

console.log(max);
// expected output: 7

const min = Math.min.apply(null, numbers);
console.log(min);
// expected output: 2
```
- The apply() method calls a function with a given this value, and arguments provided as an array (or an array-like object).
- The call() method takes arguments separately.
- The apply() method takes arguments as an array.

### bind()
```
const module = {
  x: 42,
  getX: function() {
    return this.x;
  }
};

const unboundGetX = module.getX;
console.log(unboundGetX()); // The function gets invoked at the global scope
// expected output: undefined

const boundGetX = unboundGetX.bind(module);
console.log(boundGetX());
// expected output: 42
```
- The bind() method creates a new function that, when called, has its this keyword set to the provided value, with a given sequence of arguments preceding any provided when the new function is called.

### Callbacks
```
function myDisplayer(some) {
  document.getElementById("demo").innerHTML = some;
}

function myCalculator(num1, num2, myCallback) {
  let sum = num1 + num2;
  myCallback(sum);
}

myCalculator(5, 5, myDisplayer);
```
- A callback is a function passed as an argument to another function.

### Promise
```
let myPromise = new Promise(function(myResolve, myReject) {
// "Producing Code" (May take some time)

  myResolve(); // when successful
  myReject();  // when error
});

// "Consuming Code" (Must wait for a fulfilled Promise)
myPromise.then(
  function(value) { /* code if successful */ },
  function(error) { /* code if some error */ }
);
```
- The Promise object supports two properties: state and result.
- While a Promise object is "pending" (working), the result is undefined.
- When a Promise object is "fulfilled", the result is a value.
- When a Promise object is "rejected", the result is an error object.

### Async/Await
```
async function myFunction() {
  return "Hello";
}
```
```
let value = await promise;
```
```
async function myDisplay() {
  let myPromise = new Promise(function(resolve, reject) {
    resolve("I love You !!");
  });
  document.getElementById("demo").innerHTML = await myPromise;
}

myDisplay();
```
- async makes a function return a Promise
- await makes a function wait for a Promise
- The await keyword can only be used inside an async function.
- The two arguments (resolve and reject) are pre-defined by JavaScript.
- Very often we will not need a reject function.

## javascript - Algorithm
### Remove Duplicate
```
function removeDuplicate(arr){
  var exists ={},
      outArr = [], 
      elm;

  for(var i =0; i<arr.length; i++){
    elm = arr[i];
    if(!exists[elm]){
      outArr.push(elm);
      exists[elm] = true;
   }
  }
  return outArr;
}
```
```
**Output:**
removeDuplicate([1,3,3,3,1,5,6,7,8,1]);
  = [1, 3, 5, 6, 7, 8]
  ```
### Fibonacci
#### Example - 1
```
function fibonacci(n){
  var fibo = [0, 1];
  
  if (n <= 2) return 1;

  for (var i = 2; i <=n; i++ ){
   fibo[i] = fibo[i-1]+fibo[i-2];
  }

 return fibo[n];
} 

**Output:**
fibonacci(12); // 144
```
#### Example - 2
```
function fibonacci(n){
  if(n<=1)
    return n;
  else
    return fibonacci(n-1) + fibonacci (n-2);  
}

**Output:**
fibonacci(12); // 144
```
