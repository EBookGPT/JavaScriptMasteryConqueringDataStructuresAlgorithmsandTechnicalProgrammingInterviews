# Chapter 23: Sorting Algorithms in JavaScript

Welcome back, JavaScript masters! We hope you are ready to dive into sorting algorithms, one of the most important topics in computer science. But before we start, let's quickly recap what we learned in the previous chapter.

In Chapter 22, we explored the Hash Table data structure, which is widely used in many applications such as databases, caches, and symbol tables. We learned how hash tables work, how collisions can occur, and how to handle them effectively. We also discussed the pros and cons of different hash table implementations and how to choose the right one for a specific problem.

Now, let's move on to sorting algorithms. Sorting is the process of arranging elements in a specific order, such as numerical or alphabetical order. It is a fundamental operation that is used in a wide variety of applications, from searching and data analysis to operating systems and databases.

There are many sorting algorithms available, each with its own strengths and weaknesses. In this chapter, we will explore some of the most common sorting algorithms used in practice, such as bubble sort, insertion sort, merge sort, and quicksort. We will analyze their time and space complexity, see how they are implemented in JavaScript, and compare their performance.

As always, we will provide you with plenty of code examples and exercises to help you master the material. By the end of this chapter, you will have a solid understanding of sorting algorithms and be able to solve complex sorting problems with ease.

So let's get started on our journey to JavaScript mastery with sorting algorithms!
# Chapter 23: Sorting Algorithms in JavaScript Exercises

Great job on making it this far, JavaScript mastery is within your grasp! In this exercise section, you will get to practice and apply the knowledge you have learned from the chapter on sorting algorithms.

## Exercise 1: Bubble Sort
Implement the bubble sort algorithm in JavaScript. Make sure to handle both ascending and descending orders, and to return a new sorted array without modifying the original array. Analyze the time and space complexity of your implementation.

## Exercise 2: Insertion Sort
Implement the insertion sort algorithm in JavaScript. Like the previous exercise, handle both ascending and descending orders and return a new sorted array. Analyze the time and space complexity.

## Exercise 3: Merge Sort
Implement the merge sort algorithm in JavaScript. As usual, handle both ascending and descending orders and return a new sorted array. Analyze the time and space complexity.

## Exercise 4: Quicksort
Implement the quicksort algorithm in JavaScript. Handle both ascending and descending orders and return a new sorted array. Analyze the time and space complexity.

## Exercise 5: Sorting Problems
Solve the following sorting problems using the algorithms you have just implemented:
- Sort an array of integers in non-decreasing order using bubble sort.
- Sort an array of strings in non-increasing order using insertion sort.
- Sort an array of objects by a specific property using merge sort.
- Sort an array of complex objects by multiple properties using quicksort.

## Exercise 6: Performance Comparison
Compare the performance of the four algorithms you have implemented on different array sizes (e.g., 10, 100, 1000, 10000). Use the console's performance API to measure the time each algorithm takes to sort an array. Plot the results in a chart and draw your own conclusions.

Good luck and have fun! Don't forget to check out the solutions in the appendix to compare them with your own.
## Explanation of Code for Exercise 1: Bubble Sort

In this exercise, we are asked to implement the bubble sort algorithm in JavaScript, handle both ascending and descending orders, and return a new sorted array without modifying the original array. Let's break down the code solution step by step:

```javascript
function bubbleSort(arr, order = 'ascending') {
  const n = arr.length;

  for (let i = 0; i < n - 1; i++) {
    for (let j = 0; j < n - i - 1; j++) {
      const isOutOfOrder =
        order === 'ascending' ? arr[j] > arr[j + 1] : arr[j] < arr[j + 1];

      if (isOutOfOrder) {
        const temp = arr[j];
        arr[j] = arr[j + 1];
        arr[j + 1] = temp;
      }
    }
  }

  return arr;
}
```

We first define our function `bubbleSort` and its parameters: `arr`, which is the array to be sorted, and `order`, a flag that determines whether to sort in ascending or descending order. We set `order` to `'ascending'` by default.

Next, we create a variable `n` to store the length of `arr`. This helps us keep track of how many elements are in the array, and is used later in the sorting algorithm.

We then begin our double `for` loop to iterate over each element in `arr`. The outer loop `i` runs for `n - 1` times, since we only need to compare up to the second-to-last element with the last element. The inner loop `j` runs for `n - i - 1` times, since after each iteration of the outer loop, the largest unsorted element gets bubbled up to the end, so we don't need to check it again.

Inside the inner loop, we have a conditional statement that determines whether the current pair of elements is in the wrong order, based on the value of `order`. If `order` is `'ascending'`, we check if the current element is greater than the next element. If it is, we swap them by storing the current element in a temporary variable `temp`, assigning the next element to the current position, and assigning `temp` to the next position. If `order` is `'descending'`, we simply reverse the comparison operator.

Finally, we return the sorted `arr`.

This implementation of bubble sort has a time complexity of O(n²), since it involves two nested loops. However, it has a space complexity of O(1), since it only modifies the original array in-place and uses a constant amount of extra space.


[Next Chapter](24_Chapter24.md)