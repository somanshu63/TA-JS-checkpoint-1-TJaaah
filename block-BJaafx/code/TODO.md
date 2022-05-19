1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
function average(num) {
  let result = 0;
  for(let i = 1; i <= 10; i++){
    num = +prompt("enter number");
    result = result + num;
  }
  let average = result / 10;
  return average;
}
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
// println is not defined to return the output so there will be no output instead it will show an error

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
function getEvenSum(max = 10) {
  let result = 0;
  for(let i =1; i <= max; i++){
    if(i % 2 == 0){
      result = result + i;
    }else {}
  }
  return result;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
function getOddSum(max = 10) {
  let result = 0;
  for(let i =1; i <= max; i++){
    if(i % 2 != 0){
      result = result + i;
    }else {}
  }
  return result;
}
```


5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.
```js
function getProductOfDigits(n) {
  if(n > 0){let product = 1;
    while (n != 0)
    {
        product = product * (n % 10);
        n = Math.floor(n / 10);
    }
    return product;
  } else {
    return `not a valid input`;
  }
}
```

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

check(10); // 'Bigger than 5'
check(1); // 'Smaller than 5'
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya'
getOutput('John'); // 'You are john'
getOutput(); // 'Who are you'
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // 'Who are you'
getOutput('John'); // 'Who are you'
getOutput(); // 'Who are you'
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
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
```
///this is the example which shows different output through return statement for different conditions but in a single function which shows a function can have multiple return statements

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
Command	The structure of for loop is – for(initial condition; number of iterations){//body of the loop }
Structure of while loop is-      While(condition){statements;//body}

Iterations in for loop	        Iterates for a preset number of times.	
Iterations in while loop        Iterates till a condition is met.

Condition of for loop ---	      In the absence of a condition, the loop iterates for an infinite number of times till it reaches break command.	
condition of while loop ---     In the absence of a condition, while loop shows an error.

Initialization of for loop     	Initialization in for loop is done only once when the program starts.	Initialization of while loop    Initialization is done every time the loop is iterated.

Use of for loop                	Used to obtain the result only when the number of iterations is known.	use of while loop               Used to satisfy the condition when the number of iterations is unknown.