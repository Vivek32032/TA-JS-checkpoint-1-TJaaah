1. Using loops take 10 inputs from user and find the average of all the numbers.
sum=0;
for (let i=0; i<10; i++){
let number = prompt(`Enter numbers to get the average`);
sum += Number(number);
}
console.log(sum);
let avg = sum /10;
console.log(avg);


2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}

//this will through an error as println is not defined as their is no any keyword like println in javascript. instead we can use alert or console.log to show message.
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
let sum = 0;
function getEvenSum(max = 10){
for (let i=0;i< max; i++){
  if(i%2 === 0){
    sum += i;
  } 
}
} console.log(sum);

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
 let sum = 0;
function getOddSum(max = 10){
for (let i=0;i < max; i++){
  if(i%2 !== 0){
    sum += i;
  } 
}console.log(sum);
} 

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.
function getProductOfDigits(num){
  if (num > 0){
    let result = 1
    while(num > 0){
      result =result*(num%10);
      num=Math.floor(num/10);
    } return(`result is ${result}`);
  }
  else{ return `not a valid input`;
  }
} 

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // output   `Bigger than 5`
check(1); // output    `smaller than 5`
check(5); // output     5

if num is greater it is returning `Bigger than 5` and num is smaller than 5 it is returning `smaller than 5` and by default it is returning entered argument
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // if passed argument is equal to `Arya` it will return `You are arya`
getOutput('John'); // if passed argument is equal to `John` it will return `You are John`
getOutput(); // if no argument is passed by defalut it will return `Who are you`
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // here we will get `Who are You` as an output as only this will return in all condition.
getOutput('John'); // what will be the output
getOutput(); // what will be the output
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
```js
function getSum(numA, numB){
  return numA+numB;
  return numA+1;
}
//here only first return will execute after that it comes out of function so second return statement will not run.
```
10.  What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.


In for loop, the number of iterations to be conducted is already known whereas in while loop the number of iterations are not known.

For loop contains only a single condition whereas while loop may contain a set of commands to be executed together.

In for loop, initialization of command is done only once but in while loop initialization of command is needed each time the iteration of command is done.

If the condition is absent in for loop, the loop iterates for an infinite number of times whereas the while loop shows an error in case of the absence of the condition.

For loop can be used only in case of a known number of iterations whereas while loop is used only when the number of iterations is not known.

ex :- buy a phone till you have money ,
here iteration is not known that how many times we have to run the loop only condition is given that loop will run till we money is left.

ex -2 :- print first 10 natural numbers here it is fix that we have to run the loop for 10 times so we will use while loop here.