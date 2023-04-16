# Chapter 9: Objects in JavaScript

Welcome back, JavaScript developers! In the last chapter of our book, we learned about one of the most fundamental data structures in JavaScript - arrays. In this chapter, we will delve into another critical data structure that enables us to organize and manipulate complex pieces of data - objects.

But before we get started, we have a special guest to introduce - Douglas Crockford. He is a renowned computer programmer and author, known for his contributions to the development of the JavaScript language. Crockford has a vast knowledge of JavaScript, and we are honored to have him impart his wisdom on this exciting chapter.

Objects are an essential part of JavaScript since they allow us to store and access data in a structured manner. With the help of objects, developers can create complex data structures, simulate real-world scenarios, and manipulate data with ease. We must understand this data structure if we want to master JavaScript and perform optimally during technical programming interviews.

In this chapter, we will learn how to create, manipulate, and access data stored in objects using various techniques like object properties, object methods, object constructors, and object prototypes. We will also explore different object patterns, essential object methods, and object-oriented programming concepts that are crucial for every JavaScript developer to understand.

If you're ready to learn how to conquer the world of JavaScript with mastery, then let's dive into the dynamic and exciting world of JavaScript objects!
# Chapter 9 Exercises: Objects in JavaScript

Congratulations on making it this far in our journey towards mastering JavaScript! In this chapter, we will be introducing you to the world of JavaScript objects, and equipping you with the knowledge and skills needed to work with them efficiently.

While reading through this chapter, you will encounter various key concepts that are essential in developing a deep understanding of JavaScript objects. You will come face to face with the following concepts:

- Creating Objects
- Accessing Object Data with Dot Notations
- Accessing Object Data with Bracket Notations
- Adding Properties to Objects
- Accessing Properties of Nested Objects
- Deleting Properties from Objects
- Property Enumeration
- Object Constructors
- Object Prototypes
- Object Inheritance

At the end of each sub-section, we will provide you with thought-provoking exercises that will challenge your understanding of the concepts covered in that particular sub-section. We advise you to attempt each exercise independently before referring to the answer key provided at the end of this chapter.

Our special guest in this chapter - Douglas Crockford - will enlighten you with his expert opinions on topics such as Object Patterns, Object-Oriented Design, Object Methods, and much more.

We understand that working with JavaScript objects can be challenging, but with dedicated practice, these concepts will become routine. So, without further ado, let's embark on the journey of conquering JavaScript with mastery!
Sure, let me explain the code used to resolve one of the sub-sections of Chapter 9: Objects in JavaScript.

## Using Dot Notation to Access Object Properties

In JavaScript, we can use dot notation to access the properties of an object. For instance, if we have an `Person` object that contains information about a person's name and age, we can access the name and age of the person using the following code:

```javascript
const Person = { 
  name: 'John Doe',
  age: 25 
};

console.log(Person.name); 
console.log(Person.age);
```

The `.` operator is used to signify the name of the property we want to access in the object. When we use dot notation to access a property, we must provide the property key as a string without the quotes.

We can also use dot notation to update the values of the object properties as shown below:

```javascript
Person.name = 'Jane Smith';
Person.age = 30;

console.log(Person.name); // Output: 'Jane Smith'
console.log(Person.age); // Output: 30
```

In the above code, we updated the person's name and age, and they were reflected correctly as expected.

Here is an exercise to help reinforce your understanding of accessing object properties using dot notation:

### Exercise

1. Declare an `Animal` object with the properties `name`, `type`, and `age`.
2. Console log the `name` and `type` properties of `Animal`.
3. Update the `age` property of `Animal`.
4. Console log the `age` property of `Animal`.

Good luck, and happy coding!


[Next Chapter](10_Chapter10.md)