# Chapter 5: Control Structures in JavaScript

Welcome to the fifth chapter of our book on JavaScript Mastery! In the previous chapter, we focused on the various data types in JavaScript. Now that you have a solid understanding of JavaScript data types, it's time to explore ways to control the flow of your program's execution.

In this chapter, we will introduce you to control structures in JavaScript. Control structures are an important part of any programming language, and JavaScript is no exception. They allow you to take control of how your program is executed, by specifying what code should be run under certain conditions.

We are excited to introduce our special guest for this chapter, Kyle Simpson. Kyle is a renowned JavaScript expert and the author of the book "You Don't Know JS". He has years of experience in teaching and mentoring aspiring programmers, and we are thrilled to have him share his expertise with us.

Together, we will guide you through the core concepts of control structures in JavaScript. We will explore how to use conditional statements, loops, and other control structures to make your code more efficient and effective. 

As always, we will provide you with practical examples and code samples that you can modify and test on your own. We want to ensure that you are not just learning the theory but also able to apply it in real-world scenarios.

So, roll up your sleeves and get ready to take control of your JavaScript programs with our guidance and Kyle's expertise!
# Chapter 5: Control Structures in JavaScript - Exercises

Congratulations on completing the fifth chapter of our book on JavaScript Mastery! In this chapter, we explored control structures in JavaScript and learned how to use them to control the flow of program execution. We hope you found the chapter informative and helpful.

Now, it's time to put your new skills to the test with these exercises. We have designed these exercises to reinforce the concepts covered in this chapter and test your understanding of control structures in JavaScript.

## Exercise 1: If statements

1. Write a JavaScript function that takes a number as an argument and returns whether or not the number is even.
2. Write a JavaScript function that takes a string as an argument and returns whether or not the string is empty.

## Exercise 2: Loops

1. Write a JavaScript function that takes an array of numbers and returns the sum of all the numbers in the array.
2. Write a JavaScript function that takes an array of strings and returns a new array with all the strings reversed.

## Exercise 3: Control structures in action

1. Write a JavaScript function that takes a number as an argument and returns "Fizz" if the number is divisible by 3, "Buzz" if the number is divisible by 5, and "FizzBuzz" if the number is divisible by both 3 and 5. If the number is not divisible by either 3 or 5, return the number.
2. Write a JavaScript function that takes an array of numbers and returns a new array with only the even numbers from the original array.

We encourage you to try these exercises on your own first. If you get stuck, don't worry! We have included sample solutions to each exercise in Chapter 5's GitHub repository.

We would like to thank our special guest Kyle Simpson for sharing his expertise with us in this chapter. We hope you enjoyed learning about control structures in JavaScript as much as we enjoyed teaching it to you.
## Exercise 1: If statements

### 1. Write a JavaScript function that takes a number as an argument and returns whether or not the number is even.

```javascript
function isEven(num) {
  if(num % 2 === 0) {
    return true;
  }
  else {
    return false;
  }
}
```

This function takes a number as an argument and checks if it is even or odd. It does this by checking if the number is divisible by 2. If the number is evenly divisible by 2, the remainder when divided by 2 will be 0, so the function returns `true`. Otherwise, it returns `false`.

### 2. Write a JavaScript function that takes a string as an argument and returns whether or not the string is empty.

```javascript
function isEmpty(string) {
  if(string === '') {
    return true;
  }
  else {
    return false;
  }
}
```

This function takes a string as an argument and checks if it is empty. It does this by checking if the string is equal to an empty string. If the string is empty, the function returns `true`. Otherwise, it returns `false`.

In both of these functions, we use an `if` statement to perform a conditional check. The `if` statement checks whether the condition in the parentheses is true or false. If it is true, the code inside the statement's curly braces is executed. If it is false, the code inside the `else` statement's curly braces is executed (if an `else` statement is present). The `return` statement is used to return a value from the function.


[Next Chapter](06_Chapter06.md)