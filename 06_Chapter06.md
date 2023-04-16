# Chapter 6: JavaScript Loops

Congratulations on making it to Chapter 6 of "JavaScript Mastery: Conquering Data Structures, Algorithms, and Technical Programming Interviews." In the previous chapter, we learned about control structures in JavaScript, which enable us to determine the order in which statements are executed in our programs. In this chapter, we will focus on loops, which are an essential tool in programming that allow us to execute a block of code repeatedly.

Loops come in handy when we need to execute a set of instructions multiple times under certain conditions. For example, let's say we want to print the numbers from 1 to 10. Instead of writing console.log(1); console.log(2); and so on 10 times, we can use a loop like the **for loop** to iterate through the numbers for us.

Loops come in different flavors, each with its own syntax and use case. In this chapter, we will cover the three main types of loops in JavaScript:

- The **for loop** - used for iterating over a range of numbers or elements in an array
- The **while loop** - used for executing a block of code as long as a condition is true
- The **do-while loop** - a variant of the while loop that executes the code block at least once, even if the condition is false

We will go into detail on how to use each of these loops, and provide examples to help you understand the concepts better. We will also cover some common pitfalls to avoid when using loops.

As usual, we will include code snippets throughout the chapter to make it easier for you to follow along. We encourage you to try out the examples yourself and experiment with different variations. By the end of this chapter, you should feel confident using loops in your JavaScript programs. Let's get started!
# Chapter 6 Solutions: JavaScript Loops

## Question 6.1 - Reversing a String

***Problem:*** Write a function to reverse a given string using a loop.

***Example:***
```
Input: 'hello'
Output: 'olleh'
```

***Solution:***
```javascript
function reverseString(str) {
  let reversedString = '';
  
  for(let i = str.length - 1; i >= 0; i--) {
    reversedString += str[i];
  }
  
  return reversedString;
}
```

***Explanation:***
The function `reverseString` takes in a string argument `str`, and initializes an empty string `reversedString`. We then use a `for` loop to iterate over `str` in reverse order, using the `length` property of the string minus 1 as the initial value of `i`, and decrementing `i` by 1 each iteration until it reaches 0. Inside the loop, we append the character at index `i` to `reversedString`. Finally, we return `reversedString`.

## Question 6.2 - FizzBuzz

***Problem:*** Write a function that prints the numbers from 1 to a given number. For multiples of 3, print "Fizz" instead of the number, and for multiples of 5, print "Buzz". For numbers that are multiples of both 3 and 5, print "FizzBuzz".

***Example:***
```
Input: 15
Output:
1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
FizzBuzz
```

***Solution:***
```javascript
function fizzBuzz(num) {
  for(let i = 1; i <= num; i++) {
    if(i % 3 === 0 && i % 5 === 0) {
      console.log('FizzBuzz');
    } else if(i % 3 === 0) {
      console.log('Fizz');
    } else if(i % 5 === 0) {
      console.log('Buzz');
    } else {
      console.log(i);
    }
  }
}
```

***Explanation:***
The function `fizzBuzz` takes in a number argument `num`, and uses a `for` loop to iterate over the numbers from 1 to `num`. Inside the loop, we use a series of `if` statements to check if the current number is a multiple of 3, 5, or both. If it is, we print "Fizz", "Buzz", or "FizzBuzz" accordingly. If it is not a multiple of either, we simply print the number.
## Question 6.1 - Reversing a String

The problem statement asks us to write a function to reverse a given string using a loop. We can solve this by using a `for` loop to iterate through the string in reverse order, then concatenating each character to a new string. 

Here is the breakdown of the solution:

```javascript
function reverseString(str) {
  let reversedString = '';  // Initialize an empty string to store the reversed string
  
  for(let i = str.length - 1; i >= 0; i--) {  // Start from the last character of the string and iterate backwards
    reversedString += str[i];  // Append each character to the reversedString variable
  }
  
  return reversedString;  // Return the reversed string
}
```

We define a function called `reverseString` that takes in a single string argument `str`. We then initialize an empty string variable called `reversedString` to store the reversed string.

Next, we use a `for` loop to iterate over the characters in `str` in reverse order. We start at the last character in the string (i.e. the character at index `str.length - 1`) and decrement `i` by 1 on each iteration until it reaches 0. Inside the loop, we use the `+=` operator to concatenate the current character to `reversedString`.

Finally, the function returns `reversedString`.

Here's an example of how we can call the `reverseString` function on the `'hello'` string:

```javascript
const reversed = reverseString('hello');
console.log(reversed); // Output: 'olleh'
```

This should log `'olleh'` to the console, which is the reversed version of `'hello'`.


[Next Chapter](07_Chapter07.md)