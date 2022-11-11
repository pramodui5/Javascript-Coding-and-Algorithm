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
```
**Output:**
```
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
```
**Output:**
```
fibonacci(12); // 144
```
### Swap number without temp
```
function swapNumb(a, b){
  console.log('before swap: ','a: ', a, 'b: ', b);
  b = b -a;
  a = a+ b;
  b = a-b;
  console.log('after swap: ','a: ', a, 'b: ', b);  
}
```
**Output:**
```
swapNumb(2, 3);
   = before swap:  a:  2 b:  3
   = after swap:  a:  3 b:  2
```

### String reverse
#### Example - 1
```
function reverse(str){
  var rtnStr = '';
  for(var i = str.length-1; i>=0;i--){
    rtnStr +=str[i];
  }
  return rtnStr;
}
```
Output:
```
reverse('you are a nice dude');
  = "edud ecin a era uoy"
```

#### Example - 2
```
function reverse(str){
  if(!str || str.length <2) return str;
  
  return str.split('').reverse().join('');
}
```

#### Example - 3
```
function reverse(str){
  var rtnStr = [];
  if(!str || typeof str != 'string' || str.length < 2 ) return str;
  
  for(var i = str.length-1; i>=0;i--){
    rtnStr.push(str[i]);
  }
  return rtnStr.join('');
}
```
### Reverse words
A quick solution with build in methods:
```
function reverseWords(str){
  return str.split(' ').reverse();
}
```
### Check palindrome
#### Example -1
```
function isPalindrome(str){
  var i, len = str.length;
  for(i =0; i<len/2; i++){
    if (str[i]!== str[len -1 -i])
       return false;
  }
  return true;
}
```
Output:
```
isPalindrome('madam'); // true
isPalindrome('toyota'); // false
```
#### Example - 2
Using build in method
```
function checkPalindrom(str) {
    return str == str.split('').reverse().join('');
}  
```
### Check Prime
```
function isPrime(n){
  var divisor = 2;
  while (n > divisor){
    if(n % divisor == 0){
     return false; 
    }
    else
      divisor++;
  }
  return true;
}
```
Output:
```
isPrime(137); // true
isPrime(237); // false
```

### Prime Factors
```
function primeFactors(n){
  var factors = [], 
      divisor = 2;
  
  while(n>2){
    if(n % divisor == 0){
       factors.push(divisor); 
       n= n/ divisor;
    }
    else{
      divisor++;
    }     
  }
  return factors;
}
```
Output:
```
primeFactors(69); // [3, 23]
```

### Missing number
```
function missingNumber(arr){
  var n = arr.length+1, 
  sum = 0,
  expectedSum = n* (n+1)/2;
  
  for(var i = 0, len = arr.length; i < len; i++){
    sum += arr[i];
  }
  
  return expectedSum - sum;
}
```
Output:
```
missingNumber([5, 2, 6, 1, 3]); // 4
```
### Sum of two
```
function sumFinder(arr, sum){
  var len = arr.length;
  
  for(var i =0; i<len-1; i++){  
     for(var j = i+1;j<len; j++){
        if (arr[i] + arr[j] == sum)
            return true;
     }
  }
  
  return false;
}
```
Output:
```
sumFinder([6,4,3,2,1,7], 9); // true
sumFinder([6,4,3,2,1,7], 2); // false
```

### Counting Zeros
```
function countZero(n){
  var count = 0;
  while(n>0){
   count += Math.floor(n/10);
   n = n/10;
  }
  return count;
}
```
Output:
```
countZero(2014); // 223
```

### factorialize a number
```
function factorialize(num) {
  if (num < 0) {
    return -1;
  }
  else if (num == 0){    
    return 1;
  }
  else {
    return (num * factorialize(num - 1));
  }
}

var factorial = factorialize(5)
console.log(factorial);
```
### Longest Word in a String
#### Example - 1
```
function findLongestWordLength(str) {
  var wordOne = str.split(' ');
  var maxLength = 0;
  for(var i = 0; i < wordOne.length; i++){
    if(wordOne[i].length > maxLength){
      maxLength = wordOne[i].length;
    }
  }
  return maxLength;
}

var MaxWordLength = findLongestWordLength("this is Pramod")

console.log(MaxWordLength);
```
#### Example - 2
```
function findLongestWordLength(str) {
  let arrStr =  str.split(' ');
  let longWord = 0;
  for ( let item of arrStr) {
    if(item.length > longWord) {
      longWord = item.length;
    }
  }
  return longWord
}

findLongestWordLength("word such as otorhinolaryngology");
```

### Callback Example 
```
function modifyArray(arr, callback) {
  // do something to arr here
  arr.push(100);
  // then execute the callback function that was passed
  callback();
}

var arr = [1, 2, 3, 4, 5];

modifyArray(arr, function() {
  console.log("array has been modified", arr);
});

//Output: [1,2,3,4,5,100]
```
### Reverse each word in the sentence
```
var string = "Welcome to this Javascript Guide!";

// Output becomes !ediuG tpircsavaJ siht ot emocleW
var reverseEntireSentence = reverseBySeparator(string, "");

// Output becomes emocleW ot siht tpircsavaJ !ediuG
var reverseEachWord = reverseBySeparator(reverseEntireSentence, " ");

function reverseBySeparator(string, separator) {
  return string.split(separator).reverse().join(separator);
}
```
### How to empty an array?
#### Method - 1
```
var arrayList = ['a', 'b', 'c', 'd', 'e', 'f']; // Created array
var anotherArrayList = arrayList;  // Referenced arrayList by another variable
arrayList.length = 0; // Empty the array by setting length to 0
console.log(anotherArrayList); // Output []
```

#### Method - 2
```
var arrayList = ['a', 'b', 'c', 'd', 'e', 'f']; // Created array
var anotherArrayList = arrayList;  // Referenced arrayList by another variable
arrayList = []; // Empty the array
console.log(anotherArrayList); // Output ['a', 'b', 'c', 'd', 'e', 'f']
console.log(arrayList); // []
```
### Check integer
```
function isInt(num) {
  return num % 1 === 0;
}
```
Output:
```
console.log(isInt(4)); // true
console.log(isInt(12.2)); // false
console.log(isInt(0.3)); // false
```

### Create a private variable
#### Example - 1
```
function func() {
  var priv = "secret code";
}

console.log(priv); // throws error
```
#### Example - 2
```
function func() {
  var priv = "secret code";
  return function() {
    return priv;
  }
}

var getPriv = func();
console.log(getPriv()); // => secret code
```

### What is Callback?
A callback is a plain JavaScript function passed to some method as an argument or option. It is a function that is to be executed after another function has finished executing, hence the name ‘call back‘. In JavaScript, functions are objects. Because of this, functions can take functions as arguments, and can be returned by other functions.

### What is Closure?
Closures are created whenever a variable that is defined outside the current scope is accessed from within some inner scope. It gives you access to an outer function’s scope from an inner function. In JavaScript, closures are created every time a function is created. To use a closure, simply define a function inside another function and expose it.

### Built-in methods
**CharAt()** - It returns the character at the specified index.

**Concat()** - It joins two or more strings.

**indexOf()** - It returns the index within the calling String object of the first occurrence of the specified value.

**forEach()** - It calls a function for each element in the array.

**length()** - It returns the length of the string.

**pop()** - It removes the last element from an array and returns that element.

**push()** - It adds one or more elements to the end of an array and returns the new length of the array.

**reverse()** - It reverses the order of the elements of an array.

### Difference between null & undefined?
Undefined means a variable has been declared but has not yet been assigned a value. On the other hand, null is an assignment value. 
It can be assigned to a variable as a representation of no value. Also, undefined and null are two distinct types: undefined is a type itself (undefined) while null is an object.

### Error Name values in JavaScript?
There are 6 types of Error Name values. Each one of them 
is briefly explained as follows:

* Eval Error – Thrown when coming across an error in 
  eval() (Newer JS releases don’t have it)

* Range Error – Generated when a number outside the 
  specified range is used

* Reference Error – It comes into play when an undeclared 
  variable is used.

* Syntax Error – When the incorrect syntax is used, we get 
  this error

* Type Error – This error is thrown when a value outside 
  the range of data types is tried to be used.

* URI Error – Generated due to the use of illegal characters
