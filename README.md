![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Assessment for JavaScript Fundamentals

You have 20 minutes

## Instructions

Fork, clone, and npm install.

Follow the prompts below and complete each question.  You may use any resource, other than someone else in the classroom, to help you complete this assessment.

You should save your answers in this README.md file.

# Question 1

```js
var a = 2;
var b = 3;
a = b;
```

After this code executes, what are the values of a and b? Please explain your answer.

a = 3
b = 3

After the code executes, var a is assigned the value that exists in var b (which is 3). The value in var b is not changed at all. Therefore, a is now equal to 3, and b is still equal to 3.


## Question 2

```js
var c = 5;
var d = 2;
c = c + d;
```

After this code executes, what is the value of c?  Please explain what the last line of this program `c = c + d;` means.

After this code executes, what is the value of c?  Please explain what the last line of this program `c = c + d;` means.

c = 7

'c = c + d;' is assigning the variable c to the sum of the values that currently populate the variable c (5) and the variable d (2). 5 + 2 equals 7, so the new value of variable c is 7.


## Question 3

```js
var x = 4;
var y = 3;
x = y;
y = 10;
```

After this code executes, what are the values of x and y?  Please explain your answer.

In the x = y line, the variable x is reassigned to the current value of y, which is 3, so x = 3. In the next line (y = 10), the variable y is assigned a new value of 10. This doesn't affect the above line, since it already executed, so x is still equal to 3.


## Question 4

```js
var weather;
weather = "sunny";
weather === "sunny";
```

What are the values of these expressions?  Explain your answers.

The first line (var weather;) assigns a variable weather, but doesn't assign it a value - it's undefined. The second line (weather = "sunny";) is setting that variable weather a value - so now the variable weather contains a string "sunny". The third line (weather === "sunny") checks if weather is equivalent to "sunny" - if it is, the expression will evaluate to true, and if it is not, the expression will evaluate to false. Since the variable weather does in fact contain the string "sunny", the expression evaluates to true.


## Question 5

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi >= 3) {
  console.log("sushi is delicious");
}

if (x > 0) {
  console.log("sushi is tasty");
}
```

Imagine that you take the code from this question, save it to a file called `food.js`, and run `node food.js` in your Terminal.

What would be the output? Explain your answer.

You'd receive an error, since x was never defined anywhere prior to it being called. To get "sushi is tasty" to print to the console, you might want to write something along the lines of:
  else if (howMuchILikeSushi < 3) {
    console.log("sushi is tasty");
  }


## Question 6

```js
var howMuchILikeSushi = 2;

if (howMuchILikeSushi > 0) {
  console.log("sushi is tasty");
} else if (x >= 3) {
  console.log("sushi is delicious");
} else {
  console.log("I don't like sushi");
}
```

Imagine that you take the code from this question, save it to a file called `sushi.js`, and run `node sushi.js` in your Terminal.

What would be the output? Explain your answer.

The output in the console would be a string that reads "sushi is tasty". howMuchILikeSushi is equal to 2. The if/else statement is entered, and the program checks if howMuchILikeSushi is greater than 0. Since it is, the program executes what's after that condition, which is "console.log("sushi is tasty")". Nothing after that line is executed.


## Question 7

```js
//We'll learn about require later in the course
var ask = require('./ask.js');

var answer = 'not empty';

while (answer !== '' && answer !== 'SeCrEt') {
  answer = ask("Guess my secret? ");
}
```

Imagine that you take the code from this question, save it to a file called `name.js`, and run `node name.js` in your Terminal.

What would you have to type to exit the while loop?  Explain your answer.

To exit the while loop, you'd have to enter either one of the conditions that's listed after "while" - so either an empty string OR the string 'SeCrEt'.


---

Commit and push your changes.

Submit a pull request.
