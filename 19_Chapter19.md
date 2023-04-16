# Chapter 19: Tree Data Structure

Welcome to chapter 19 of JavaScript Mastery: Conquering Data Structures, Algorithms, and Technical Programming Interviews! 

In the previous chapter, we talked about the Queue data structure, which is a linear data structure that follows the First In First Out (FIFO) principle. Now, we move onto a non-linear data structure, the Tree. Trees are used in many real-world applications ranging from computer science to biology to linguistics. Today, you will gain a comprehensive understanding of trees in computer science and their applications. 

Before diving into the depths of the Tree data structure, we would like to introduce a special guest who helped pave the way for Trees as we know them today. Meet Adelson-Velsky and Landis, the computer scientists who first proposed the use of balanced binary search trees (AVL trees) in 1962. Their development of AVL trees sparked innovation and interest in tree data structures, leading to many improvements and variations that we use today.

In this chapter, we will explore the various types of trees, including Binary Trees, Binary Search Trees, AVL Trees, and Red-Black Trees. We'll also learn about tree traversal algorithms, such as the Depth-First Search (DFS) and Breadth-First Search (BFS), which are used to search and analyze trees. We'll provide real-world examples to help you understand how trees can be applied to solve problems in various domains.

No matter what type of application or domain you work in, understanding Trees is essential for mastering data structures and algorithms. By the end of this chapter, you will have a great foundation of knowledge and experience with the Tree data structure in JavaScript.

So, let's dive into the world of Trees with Adelson-Velsky and Landis guiding our way!
# Chapter 19: Tree Data Structure - Exercises

Congratulations on completing the introduction to the Tree data structure! It's time to put your knowledge to the test with these exercises.

## Exercise 1: Implement a Binary Tree in JavaScript

Create a Binary Tree Class in JavaScript that can perform the following functions:
- `insert(value)`: inserts a value into the binary tree.
- `contains(value)`: searches for a value in the binary tree and returns true if found, false if not found.
- `size()`: returns the number of nodes in the binary tree.

For example, the code below should output `true` and `false` respectively:
```
const tree = new BinaryTree();
tree.insert(10);
tree.insert(5);
tree.insert(15);
console.log(tree.contains(5)); // true
console.log(tree.contains(20)); // false
```

## Exercise 2: Implement Depth-First Search (DFS) on a Binary Tree

Write a function in JavaScript that performs Depth-First Search (DFS) on a Binary Tree and returns an array of nodes in the order they were visited. Your DFS function should accept the root node of the binary tree as a parameter.

For example, given a binary tree with a root of node `10` and left and right children with nodes `5` and `15` respectively, the DFS output for this binary tree should be `[10, 5, 15]`.

## Exercise 3: Implement Breadth-First Search (BFS) on a Binary Tree

Write a function in JavaScript that performs Breadth-First Search (BFS) on a Binary Tree and returns an array of nodes in order they were visited. Your BFS function should accept the root node of the binary tree as a parameter.

For example, given a binary tree with a root of node `10` and left and right children with nodes `5` and `15` respectively, the BFS output for this binary tree should be `[10, 5, 15]`.

## Bonus Exercise: Implement an AVL Tree

Challenge yourself by implementing an AVL Tree class in JavaScript that can perform the following functions:
- `insert(value)`: inserts a value into the AVL tree.
- `contains(value)`: searches for a value in the AVL tree and returns true if found, false if not found.
- `size()`: returns the number of nodes in the AVL tree.

An AVL Tree is a self-balancing binary search tree, meaning that at any given node, the heights of the left and right subtrees differ by at most one. 

Best of luck with the exercises! Remember to stay curious and keep practicing your skills in data structures and algorithms.
Sure, let me explain the solution to Exercise 2: Implement Depth-First Search (DFS) on a Binary Tree.

Below is an example function that performs DFS on a binary tree by recursively traversing the nodes in a pre-order manner (root, left, right). The function takes in the root node of the binary tree as a parameter:
```javascript
function dfs(node) {
  if (!node) return [];
  
  const result = [];
  
  function traverse(root) {
    if (root) result.push(root.value);
    if (root.left) traverse(root.left);
    if (root.right) traverse(root.right);
  }
  
  traverse(node);
  return result;
}
```
The `dfs` function creates an empty array `result` and a nested helper function `traverse` that recursively traverses the nodes in the binary tree. 

The `traverse` function first checks if the node passed to it is not null or undefined. If `node` is null, an empty array is returned.

Next, the function checks if `root` is not null. If `root` is not null, its value is pushed into `result`. 

Finally, the function checks if `root` has a left child or right child, and recursively calls `traverse` on each child respectively.

The `dfs` function invokes `traverse` on the root node, and returns the `result` array.

For example, given a binary tree with a root of node `10` and left and right children with nodes `5` and `15` respectively, the DFS output for this binary tree would be `[10, 5, 15]`.

I hope that helps explain the code used to resolve this exercise! Let me know if you have any further questions.


[Next Chapter](20_Chapter20.md)