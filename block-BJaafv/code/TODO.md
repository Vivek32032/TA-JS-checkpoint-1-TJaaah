1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
//first will return sum of a and b but second will return undefined as nothing is returning.


2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
// value of first is sum of a and b but second function will have undefined as nothing is returning. 

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
//if we pass 3 value in sum function it will take first two arguments as don't have third parameter.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
yes, we can store a function in a variable as we consider function as a expression.
5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
  
 ```js
function sayHello(name){
  return `Hello ${name}`;
}
```
1. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
// outpot: `Hello John`;
  as we have declared useName earlier so and this function has not any parameter so the value declared earlier will get executed .

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1 `John`

showMessage(); // Output 2  `Hello, John`

alert(userName); // Output 3 `John`
```

8. What is a Anonymous Function give example of three functions.
function do not have any name is called anonymous function.
let sayHello = function(name){
  return `Hello ${name}`;
}

let sum = function(numA, numB){
  return a+b;
}

let multiplyOfNum = function(numA, numB){
  return numA*numB;
}

1. Can function declaration be a Anonymous Function? Explain
yes, but there will be no any use of function declaration as we have assigned it to a variable.

2.  Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
"store" -store a value.
"call" -call value
"print" -print the value.
"length"- stores length of a value.
"remove" - removes a value.
"reset" -reset a value.
"puts" - puts a value.
