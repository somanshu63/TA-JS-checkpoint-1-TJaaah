1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}
//this will return the sum 
// second
function sum(a, b) {
  console.log(a + b);
}
//whereas this will log the sum and return undefined
```

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
//first = the value ie 10
second = undefined as there is no return therefore undefined is returned if there is no return expression
if we take sum(5, 5); // 10

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
//this will return the sum of first two parameters that are passed because while declarating the function only 2 parameters were passed 

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
yes like this we can store a function in a variable
const add = (a, b) => a + b;

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
function sayHello(name) {
  return `Hello ${name}`;
}

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
// output is 'Hello, John' because if function is unable to find the username inside it will go to outside to find it

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // John

showMessage(); // 'Hello, John'

alert(userName); // John
```

8. What is a Anonymous Function give example of three functions.
Anonymous Function is a function that does not have any name associated with it.
example-1
var hello = function () {
    console.log("helloworld!");
};
example-2
var station = function (platform) {
    console.log("Welcome to ", platform);
};
example-3
const showmessage = function() {
  let message = 'Hello, ' + userName;
  return message;
}

9. Can function declaration be a Anonymous Function? Explain
yes 
example-
const showmessage = function() {
  let message = 'Hello, ' + userName;
  return message;
}
in this function is declared but without name so it will be called anonymous function declaration


10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

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

"add" - add values
"calculateBmi" - calculates the bmi
"appropriateDrinks" - tells which drink is for which age
"isInRange" - tells wheather the value is in range or not
 "minToSec" - converts minutes to secs
