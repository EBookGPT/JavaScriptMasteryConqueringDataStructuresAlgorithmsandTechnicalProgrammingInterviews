# Chapter 2: Fundamentals of JavaScript

Welcome back, aspiring JavaScript Masters! In the previous chapter, we discussed the introduction to JavaScript Mastery, and now it's time to dive into the nitty-gritty of this powerful programming language.

Today, we have a special guest with us, none other than Kyle Simpson, a well-known JavaScript expert, and author of the book "You Don't Know JS". He is here to provide his insights and expertise on the topic, and I am sure we all will benefit greatly from his wisdom.

As you all know, JavaScript is a programming language that is used extensively in web development. The language has incredible potential and versatility, but to truly master it, we must first start with the basics.

In this chapter, we will go over the fundamental concepts of JavaScript, including:

- Variables and Data Types
- Operators
- Loops and Iteration
- Conditional Statements
- Functions and Scoping

We will start by discussing the basics of JavaScript syntax and data types. Once we have a solid understanding of these building blocks, we will then move on to cover operators and control structures. We will also learn about functions, their purpose, and how to use them to write efficient and reusable code.

By the end of this chapter, you will have a solid foundation in JavaScript Fundamentals, which will help you in your journey towards becoming a JavaScript Master. So let's get started! 

And a huge thank you to Kyle Simpson for joining us and his valuable contributions to this chapter.
# Chapter 2 Homework: Fundamentals of JavaScript

Congratulations on completing Chapter 2 of the "JavaScript Mastery" textbook! In this chapter, you explored the foundational concepts of JavaScript programming, including variables, data types, operators, loops, conditional statements, functions, and scoping.

To help reinforce your understanding of these concepts, we have provided a set of practice problems for you to solve. These problems range in difficulty, so you can start with the easier ones and work your way up to the more challenging ones.

But before we dive into the problems, we would like to thank our special guest, Kyle Simpson, for joining us in this chapter. His insights and expertise on JavaScript fundamentals were invaluable, and we are lucky to have had him share his knowledge with us.

Without further ado, let's jump into the problems! Each problem contains a description and some starter code. Your task is to complete the code and write a working solution in JavaScript.

## Problem 1: Reverse a String

Write a function called `reverseString` that takes a string as an argument and returns the reverse of that string.

```javascript
function reverseString(str) {
  // your code here
}

console.log(reverseString('hello')); // should return 'olleh'
```

## Problem 2: Find the Maximum Number

Write a function called `findMax` that takes an array of numbers as an argument and returns the maximum number in that array.

```javascript
function findMax(arr) {
  // your code here
}

console.log(findMax([1, 2, 3, 4, 5])); // should return 5
```

## Problem 3: Check if Two Strings are Anagrams

Write a function called `isAnagram` that takes two strings as arguments and returns `true` if the two strings are anagrams of each other and `false` otherwise.

```javascript
function isAnagram(str1, str2) {
  // your code here
}

console.log(isAnagram('listen', 'silent')); // should return true
```

## Problem 4: Return Unique Elements from an Array

Write a function called `getUnique` that takes an array of numbers as an argument and returns a new array containing only the unique elements of that array.

```javascript
function getUnique(arr) {
  // your code here
}

console.log(getUnique([1, 2, 2, 3, 3, 4, 5, 5])); // should return [1, 2, 3, 4, 5]
```

## Problem 5: Determine if Brackets are Balanced

Write a function called `balancedBrackets` that takes a string of brackets as an argument and returns `true` if the brackets are balanced and `false` otherwise. For example, `balancedBrackets("[()]{}{[()()]()}")` should return `true`.

```javascript
function balancedBrackets(str) {
  // your code here
}

console.log(balancedBrackets("[()]{}{[()()]()}")); // should return true
```

Great job on completing these practice problems! Keep practicing and honing your JavaScript skills, and you will be well on your way towards JavaScript Mastery.
Certainly! Let's take a look at the five problems and their solutions from the previous section:

## Problem 1: Reverse a String

```javascript
function reverseString(str) {
  // Step 1. Use the split() method to return a new array
  var splitString = str.split(''); // var splitString = 'hello'.split('');
  // ["h", "e", "l", "l", "o"]
 
  // Step 2. Use the reverse() method to reverse the new created array
  var reverseArray = splitString.reverse(); // var reverseArray = ["h", "e", "l", "l", "o"].reverse();
  // ["o", "l", "l", "e", "h"]
 
  // Step 3. Use the join() method to join all elements of the array into a string
  var joinArray = reverseArray.join(''); // var joinArray = ["o", "l", "l", "e", "h"].join('');
  // "olleh"
  
  // Step 4. Return the reversed string
  return joinArray; // "olleh"
}
```
This problem can be solved by using the `split()`, `reverse()`, and `join()` methods of the `String` object. First, we convert the input string into an array of separate characters using the `split()` method. We then use the `reverse()` method to reverse the order of the array elements. Finally, we concatenate the reversed array elements into a new string using the `join()` method.

## Problem 2: Find the Maximum Number

```javascript
function findMax(arr) {
  // Step 1. Use the apply() method to pass the array elements to the Math.max() method as arguments
  return Math.max.apply(null, arr);
}

console.log(findMax([1, 2, 3, 4, 5])); // should return 5
```

This problem can be solved by using the `apply()` method of the `Math` object. The `apply()` method allows us to invoke a function with an array of arguments passed to it. In this case, we pass the entire array of numbers to the `Math.max()` method, which returns the maximum value in the array.

## Problem 3: Check if Two Strings are Anagrams

```javascript
function isAnagram(str1, str2) {
  // Step 1. Use the split() method to return two new arrays
  var arr1 = str1.split('');
  var arr2 = str2.split('');

  // Step 2. Sort the arrays
  arr1.sort();
  arr2.sort();

  // Step 3. Compare the sorted arrays
  for(var i = 0; i < arr1.length; i++) {
    if(arr1[i] !== arr2[i]) {
      return false;
    }
  }

  return true;
}

console.log(isAnagram('listen', 'silent')); // should return true
```

This problem can be solved by splitting both input strings into arrays of characters and then sorting those arrays. Finally, we compare each element of the two sorted arrays. If all the elements match, then the strings are anagrams of each other.

## Problem 4: Return Unique Elements from an Array

```javascript
function getUnique(arr) {
  // Step 1. Use the filter() method to return a new array with unique elements
  var uniqueArray = arr.filter(function(item, pos) {
    return arr.indexOf(item) == pos;
  });

  return uniqueArray;
}

console.log(getUnique([1, 2, 2, 3, 3, 4, 5, 5])); // should return [1, 2, 3, 4, 5]
```

This problem can be solved by using the `filter()` method of the `Array` object. The `filter()` method returns a new array with elements that pass the test specified by a callback function. In this case, we use the `indexOf()` method to locate the first occurrence of each element in the original array. If an element occurs at a different position than its first occurrence, it is filtered out.

## Problem 5: Determine if Brackets are Balanced

```javascript
function balancedBrackets(str) {
  // Step 1. Define a stack variable
  var stack = [];
  
  // Step 2. Create a lookup table for bracket pairs
  var bracketPairs = {
    '(': ')',
    '{': '}',
    '[': ']'
  };
  
  // Step 3. Loop through the string
  for(var i = 0; i < str.length; i++) {
    var char = str[i];
    
    // Step 4. Push opening brackets onto stack
    if(bracketPairs[char]) {
      stack.push(char);
    } else {
      // Step 5. Check if current character is a closing bracket
      var lastBracket = stack.pop();
      if(char !== bracketPairs[lastBracket]) {
        return false;
      }
    }
  }
  
  // Step 6. If the stack is empty after looping through the string, then brackets are balanced
  return stack.length === 0;
}

console.log(balancedBrackets("[()]{}{[()()]()}")); // should return true
```

This problem can be solved by using a stack data structure. We loop through the string of brackets, push opening brackets onto the stack, and pop them off when we encounter a corresponding closing bracket. We use a lookup table to find the matching closing bracket for each opening bracket. If the closing bracket is not the same as the last bracket on the stack, then the brackets are not balanced. If we finish looping through the string and the stack is empty, then the brackets are balanced.


[Next Chapter](03_Chapter03.md)