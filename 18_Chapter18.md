# Chapter 18: Queue Data Structure

Welcome back, Javascript Masters! In our previous chapter, we delved into the Stack data structure and explored various algorithms and operations associated with it. We hope you had a great time learning about the Stack, and we're excited to introduce you to the next topic in our series, the Queue Data Structure.

A queue is a linear data structure, much like the Stack. However, unlike the Stack that follows a LIFO (Last in First Out) approach, the Queue follows the FIFO (First in First Out) approach. This means that the element that is inserted first is the first to be removed from the Queue.

Queues find their application in many real-world scenarios, such as a Print Queue at your office, People waiting in line for tickets or rides, or even in computer algorithms such as BFS (Breadth First Search). 

To learn more about Queues, we've brought in a very special guest - Vaidehi Joshi. She is a software engineer at Tilde, co-host of the Base.cs Podcast, and author of the popular "BaseCS" blog series. With her experience and expertise, we will delve deeper into various algorithms associated with the Queue Data Structure and their implementation in Javascript.

So, let's get ready to Queue up!
# Chapter 18: Queue Data Structure

## Introduction
In the world of data structures, queues are the unsung heroes of everyday life. They’re found everywhere from your operating system to the line at Disneyland. As we all know, good things come to those who wait. With queues, this couldn’t be more true. Today we’re going to be exploring the wonderful world of queues and how they can be implemented in JavaScript. We have a special guest with us today who will guide us through the algorithms associated with queues and other intricacies. Vaidehi Joshi, software engineer at Tilde and author of the popular "BaseCS" blog series, will be joining us!

## Queue Definition
A Queue is a simple data structure that follows the FIFO (First In First Out) principle. Queues work the way a line works, where elements are added one at a time to the back, and removed one at a time from the front. A classic example of this is a Print Queue.

## Queue Operations
The key operations of a Queue include:
- `Enqueue`: Adds an element to the end of the Queue.
- `Dequeue`: Removes the first element from the Queue.
- `Front`: Returns the first element from the Queue without deleting it.
- `isEmpty`: Checks if the Queue is empty.
- `size`: Returns the number of elements in the Queue.

## Implementation in JavaScript
Queues can easily be implemented in JavaScript using arrays. You can push elements to the end of the array using the `push()` function, and remove elements from the beginning of the array using the `shift()` function. More complex Queues may be implemented using LinkedLists, where the LinkedList is used to store the elements and the `head` and `tail` pointers are used to keep track of the ends of the Queue.

## Example Code
```javascript
class Queue {
  constructor() {
    this.items = [];
  }

  enqueue(element) {
    this.items.push(element);
  }

  dequeue() {
    if (this.items.length == 0)
      return "Underflow";
    return this.items.shift();
  }

  front() {
    if (this.items.length == 0)
      return "Underflow";
    return this.items[0];
  }

  isEmpty() {
    return this.items.length == 0;
  }

  size() {
    return this.items.length;
  }
}
```
## Conclusion
With this clear understanding of Queues and their implementation in JavaScript, you can implement your own Queue data structure for your needs. Queues are used frequently in many different contexts and problems, so keep an eye out for ways to apply them in your development work. A big thank you to Vaidehi Joshi for joining us and sharing her wisdom on this important topic. Happy Queuing!
In the chapter we introduced a JavaScript implementation of the Queue data structure using class syntax. Let's explain the code in more detail:

```javascript
class Queue {
  constructor() {
    this.items = [];
  }
```
Here we define a class `Queue` that has a constructor function that sets an array `items` as the attribute of the queue. This array will hold all the elements that are added to the Queue.

```javascript
  enqueue(element) {
    this.items.push(element);
  }

  dequeue() {
    if (this.items.length == 0)
      return "Underflow";
    return this.items.shift();
  }
```
The `enqueue()` function inserts an element into the end of the `items` array. The `dequeue()` function removes the first element from the front of the array using `shift()` method. 

Note that in the `dequeue()` function, we are first checking if the array is empty, to avoid shifting undefined values.

```javascript
  front() {
    if (this.items.length == 0)
      return "Underflow";
    return this.items[0];
  }
```
The `front()` function retrieves the first element in the `items` array without deleting it. Here, we first check if the array is empty or not to avoid accessing undefined values.

```javascript
  isEmpty() {
    return this.items.length == 0;
  }

  size() {
    return this.items.length;
  }
}
```
The `isEmpty()` function returns a boolean value based on whether the `items` array is empty or not. The `size()` function returns the length of the `items` array, which provides the current size of the Queue.

This implementation is simple, but it effectively demonstrates the fundamental operations of the Queue data structure.


[Next Chapter](19_Chapter19.md)