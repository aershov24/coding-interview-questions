# 300 Coding Interview Questions (ANSWERED) To Land Your Next Six-Figure Job Offer from [FullStack.Cafe](https://www.fullstack.cafe)

[FullStack.Cafe](https://www.fullstack.cafe) is a biggest hand-picked collection of most common coding interview questions for software developers. Prepare for your next programming interview in no time and get 6-figure job offer fast!

> Yeah! 🧨 All Answers + PDF's available on [FullStack.Cafe - Kill Your Coding Interview](https://www.fullstack.cafe)!

## <a name='toc'>Table of Contents</a>
 * [Arrays](#Arrays)
 * [Backtracking](#Backtracking)
 * [Big-O Notation](#Big-ONotation)
 * [Binary Tree](#BinaryTree)
 * [Bit Manipulation](#BitManipulation)
 * [Blockchain](#Blockchain)
 * [Brain Teasers](#BrainTeasers)
 * [Divide & Conquer](#Divide&Conquer)
 * [Dynamic Programming](#DynamicProgramming)
 * [Fibonacci Series](#FibonacciSeries)
 * [Graph Theory](#GraphTheory)
 * [Greedy Algorithms](#GreedyAlgorithms)
 * [Hash Tables](#HashTables)
 * [Heaps and Maps](#HeapsandMaps)
 * [Linked Lists](#LinkedLists)
 * [Queues](#Queues)
 * [Recursion](#Recursion)
 * [Searching](#Searching)
 * [Sorting](#Sorting)
 * [Stacks](#Stacks)
 * [Strings](#Strings)
 * [Trees](#Trees)
 * [Trie](#Trie)
## [[⬆]](#toc) <a name=Arrays>Arrays</a> Interview Questions
#### Q1: Explain what is an Array? ⭐
**Answer:**
An **array** is a collection of **homogeneous** (same type) data items stored in **contiguous memory** locations. For example if an array is of type “int”, it can only store integer elements and cannot allow the elements of other types such as double, float, char etc. The elements of an array are accessed by using an **index**. 

* <code><i>O</i>(<i>1</i>)</code>
* <code><i>O</i>(<i>log n</i>)</code>
* <code><i>O</i>(<i>n</i>)</code>
* <code><i>O</i>(<i>n log n</i>)</code>
* <code><i>O</i>(<i>n</i><sup>2</sup>)</code>
* <code><i>O</i>(<i>2</i><sup>n</sup>)</code>
* <code><i>O</i>(<i>n!</i>)</code>

**Source:** _beginnersbook.com_

#### Q2: Name some characteristics of Array Data Structure ⭐
**Answer:**
Arrays are: 
* **Finite (fixed-size)** - An array is finite because it contains only limited number of elements.
* **Order** -All the elements are stored one by one , in contiguous  location of computer memory in a linear order and fashion
* **Homogenous** - All  the elements of an array are of  same  data types only  and hence  it is termed as collection of homogenous

**Source:** _codelack.com_

#### Q3: Name some advantages and disadvantages of Arrays ⭐⭐
**Answer:**
**Pros:**
* **Fast lookups**. Retrieving the element at a given index takes `O(1)` time, regardless of the length of the array.
* **Fast appends**. Adding a new element at the end of the array takes `O(1)` time.

**Cons:**
* **Fixed size**. You need to specify how many elements you're going to store in your array ahead of time.
* **Costly inserts and deletes**. You have to shift the other elements to fill in or close gaps, which takes worst-case `O(n)` time.

**Source:** _www.interviewcake.com_

#### Q4: What is time complexity of basic Array operations? ⭐⭐
**Answer:**
Array uses continuous memory locations (**space** complexity `O(n)`) to store the element so **retrieving** of any element will take `O(1)` time complexity (constant time by using index of the retrieved element). `O(1)` describes **inserting** at the end of the array. However, if you're inserting into the middle of an array, you have to shift all the elements after that element, so the complexity for insertion in that case is `O(n)` for arrays. End appending also discounts the case where you'd have to resize an array if it's full.


|Operation	|Average Case	|Worst Case
|-|-|-|
|Read	    | `O(1)`	        |`O(1)`
|Append       |`O(1)`            |`O(1)`
|Insert	   |`O(n)`	        |`O(n)`
|Delete	   |`O(n)`	        |`O(n)`
|Search	   |`O(n)`	        |`O(n)`


**Source:** _beginnersbook.com_

#### Q5: What is a main difference between an Array and a Dictionary? ⭐⭐
**Answer:**
Arrays and dictionaries both store collections of data, but differ by _how they are accessed_. Arrays provide _random access_ of a sequential set of data. Dictionaries (or associative arrays) provide a _map_ from a _set of keys_ to a _set of values_. 
* Arrays store a set of objects (that can be accessed randomly)
* Dictionaries store pairs of objects
* Items in an array are accessed by position (_index_) (often a number) and hence have an order. 
* Items in a dictionary are accessed by _key_ and are unordered.

This makes array/lists more suitable when you have a group of objects in a set (prime numbers, colors, students, etc.). Dictionaries are better suited for showing relationships between a pair of objects.

**Source:** _stackoverflow.com_

#### Q6: What are Dynamic Arrays? ⭐⭐
**Answer:**
A **dynamic array** is an array with a big improvement: _automatic resizing_.

One limitation of arrays is that they're _fixed_ size, meaning you need to specify the number of elements your array will hold ahead of time. A dynamic array expands as you add more elements. So you don't need to determine the size ahead of time.

**Source:** _www.interviewcake.com_

#### Q7: How do Dynamic Arrays work? ⭐⭐
**Answer:**
A simple dynamic array can be constructed by _allocating an array of fixed-size_, typically _larger_ than the number of elements immediately required. The elements of the dynamic array are stored contiguously at the start of the underlying array, and the remaining positions towards the end of the underlying array are reserved, or unused. Elements can be added at the end of a dynamic array in constant time by using the reserved space until this space is completely consumed.

When all space is consumed, and an additional element is to be added, the underlying fixed-sized array needs to be increased in size. Typically resizing is expensive because you have to allocate a bigger array and copy over all of the elements from the array you have overgrow before we can finally append our item.

Dynamic arrays memory allocation is language specific. For example in C++ arrays are created on the stack, and have automatic storage duration -- you don't need to manually manage memory, but they get destroyed when the function they're in ends. They necessarily have a fixed size:

```js
int foo[10];
```

Arrays created with operator `new[]` have _dynamic_ storage duration and are stored on the heap (technically the "free store"). They can have any size, but you need to allocate and free them yourself since they're not part of the stack frame:

```js
int* foo = new int[10];
delete[] foo;
```


**Source:** _stackoverflow.com_

#### Q8: What is an Associative Array? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: What are time complexities of sorted array operations? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: What does Sparse Array mean? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: When to use a Linked List over an Array/Array List? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Compare Array based vs Linked List stack implementations ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: How exactly indexing works in Arrays? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: What are advantages of Sorted Arrays? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: What is the advantage of Heaps over Sorted Arrays? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: How to merge two sorted Arrays into a Sorted Array? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: What defines the dimensionality of an Array? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: How would you compare Dynamic Arrays with Linked Lists and vice versa?  ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: Why is the complexity of fetching from an Array be <code><i>O</i>(<i>1</i>)</code>? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q20: How to implement 3 Stacks with one Array? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q21: Check for balanced parentheses in linear time using constant space ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Backtracking>Backtracking</a> Interview Questions
#### Q1: What is Backtracking? ⭐
**Answer:**
**Backtracking** is a systematic way of trying out different sequences of decisions until we find one that "works." Backtracking does not generate all possible solutions first and checks later. It tries to generate a solution and as soon as even one constraint fails, the solution is rejected and the next solution is tried.

Backtracking can be understood as as searching os a tree for a particular "goal" leaf node. Backtracking in that case is a **depth-first search** with any bounding function. All solution using backtracking is needed to satisfy a complex set of constraints.


![](https://static.javatpoint.com/tutorial/daa/images/backtracking-introduction.png)


**Source:** _www.javatpoint.com_

#### Q2: What is the difference between Backtracking and Recursion? ⭐⭐
**Answer:**
* **Recursion** describes the calling of the _same function_ that you are in. The typical example of a recursive function is the factorial. You always need a condition that makes recursion stop (base case). 
* **Backtracking** is when the algorithm makes an opportunistic decision<sup>*</sup>, which may come up to be wrong. If the decision was wrong then the backtracking algorithm restores the state before the decision. It builds candidates for the solution and abandons those which cannot fulfill the conditions. A typical example for a task to solve would be the _Eight Queens Puzzle_. Backtracking is also commonly used within _Neuronal Networks_. Many times backtracking is not implemented recursively. If backtracking uses recursion its called **Recursive Backtracking**

P.S. <sup>*</sup> **Opportunistic decision** making refers to a process where a person or group assesses alternative actions made possible by the favorable convergence of immediate circumstances recognized **without** reference to any **general plan**.

**Source:** _www.quora.com_

#### Q3: Why is this called Backtracking? ⭐⭐
**Answer:**
1. Using Backtracking you built a **solution** (that is a structure where every variable is assigned a value).
2. It is however possible that during construction, you realize that the solution is **not successful** (does not satisfy certain constraints), then you **backtrack**: you _undo_ certain assignments of values to variables in order to reassign them.

Like when looking for a book  because at first you check drawers in the first room, but it's not found, so you _backtrack_ out of the first room to check the drawers in the next room. It's also called **Trial & Error**.

**Source:** _stackoverflow.com_

#### Q4: What is Exhaustive Search? ⭐⭐
**Answer:**
**Exhaustive Search** is an algorithmic technique in which first all possible solutions are generated first and then we select the most feasible solution by applying some rules. Since it follows the most naive approach, it is a.k.a **Brute-Force Search**. This approach is one of the **most expensive** algorithmic techniques, mainly in terms of time complexity. It is also, therefore, one of the most **naive** ones.

**Source:** _afteracademy.com_

#### Q5: Explain what is DFS (Depth First Search) algorithm for a Graph and how does it work? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: Find all the Permutations of a String ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: What is the difference between Backtracking and Exhaustive Search techniques? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: Explain what is Explicit and Implicit Backtracking Constrains? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Big-ONotation>Big-O Notation</a> Interview Questions
#### Q1: What is _Big O_ notation? ⭐
**Answer:**
**Big-O** notation (also called "asymptotic growth" notation) is a relative representation of the complexity of an algorithm. It shows how an algorithm *scales* based on input size. We use it to talk about how thing _scale_. Big O complexity can be visualized with this graph:


![](https://i.stack.imgur.com/WcBRI.png)


**Source:** _stackoverflow.com_

#### Q2: Provide an example of <code><i>O</i>(<i>1</i>)</code> algorithm ⭐
**Answer:**
Say we have an array of `n` elements:

```cs
int array[n];
```

If we wanted to access the first (or any) element of the array this would be <code><i>O</i>(<i>1</i>)</code> since it doesn't matter how big the array is, it always takes the same constant time to get the first item:
```cs
x = array[0];
```

**Source:** _stackoverflow.com_

#### Q3: What is Worst Case? ⭐⭐
**Answer:**
Big-O is often used to make statements about functions that measure the worst case behavior of an algorithm. **Worst case** analysis gives the maximum number of basic operations that have to be performed during execution of the algorithm. It assumes that the input is in the _worst possible state_ and maximum work has to be done to put things right.

**Source:** _stackoverflow.com_

#### Q4: What the heck does it mean if an operation is <code><i>O</i>(<i>log n</i>)</code>? ⭐⭐
**Answer:**
**<code><i>O</i>(<i>log n</i>)</code>** means for every element, you're doing something that only needs to look at **log N** of the elements. This is usually because you know something about the elements that let you make an _efficient choice_ (for example to reduce a _search space_). 
The most common attributes of logarithmic running\-time function are that:
*   the choice of the next element on which to perform some action is one of several possibilities, and
*   only one will need to be chosen

or

*   the elements on which the action is performed are digits of `n`

Most efficient sorts are an example of this, such as **merge sort**. ​It is `O(log n)` when we do divide and conquer type of algorithms e.g binary search. Another example is **quick sort** where each time we divide the array into two parts and each time it takes `O(N)` time to find a pivot element. Hence it `N O(log N)`

Plotting `log(n)` on a plain piece of paper, will result in a graph where the rise of the curve decelerates as `n` increases:
![](https://i.stack.imgur.com/qPNNp.png)


**Source:** _stackoverflow.com_

#### Q5: Why do we use Big O notation to compare algorithms?  ⭐⭐
**Answer:**
The fact is it's difficult to determine the exact runtime of an algorithm. It depends on the speed of the computer processor. So instead of talking about the runtime directly, we use Big O Notation to talk about _how quickly the runtime grows_ depending on input size.

With Big O Notation, we use the size of the input, which we call `n`. So we can say things like the runtime grows “on the order of the size of the input” (<code><i>O</i>(<i>n</i>)</code>) or “on the order of the square of the size of the input” (<code><i>O</i>(<i>n</i><sup>2</sup>)</code>). Our algorithm may have steps that seem expensive when `n` is small but are eclipsed eventually by other steps as `n` gets larger. For Big O Notation analysis, we care more about the stuff that grows fastest as the input grows, because everything else is quickly eclipsed as `n` gets very large.

**Source:** _medium.com_

#### Q6: What exactly would an <code><i>O</i>(<i>n</i><sup>2</sup>)</code> operation do? ⭐⭐
**Answer:**
**<code><i>O</i>(<i>n</i><sup>2</sup>)</code>** means for every element, you're doing something with _every_ other element, such as comparing them. Bubble sort is an example of this.

**Source:** _stackoverflow.com_

#### Q7: What is complexity of this code snippet? ⭐⭐
**Details:**
Let's say we wanted to find a number in the list:
```js
for (int i = 0; i < n; i++){
    if(array[i] == numToFind){ return i; }
}
```
What will be the time complexity (Big O) of that code snippet?

**Answer:**
This would be <code><i>O</i>(<i>n</i>)</code> since at most we would have to look through the entire list to find our number. The Big-O is still <code><i>O</i>(<i>n</i>)</code> even though we might find our number the first try and run through the loop once because Big-O describes the upper bound for an algorithm.

**Source:** _stackoverflow.com_

#### Q8: What is complexity of `push` and `pop` for a Stack implemented using a LinkedList? ⭐⭐
**Answer:**
<code><i>O</i>(<i>1</i>)</code>. Note, you don't have to insert at the end of the list. If you insert at the front of a (singly-linked) list, they are both `O(1)`.

Stack contains 1,2,3:

```py
[1]->[2]->[3]
```

Push 5:

```js
[5]->[1]->[2]->[3]
```

Pop:

```js
[1]->[2]->[3] // returning 5
```


**Source:** _stackoverflow.com_

#### Q9: Explain the difference between _`O(1)`_ vs _`O(n)`_ space complexities  ⭐⭐
**Answer:**
Let's consider a traversal algorithm for traversing a list.

* <code><i>O</i>(<i>1</i>)</code> denotes _constant_ space use: the algorithm allocates the same number of pointers irrespective to the list size. That will happen if we move (reuse) our pointer along the list.
* In contrast, <code><i>O</i>(<i>n</i>)</code> denotes _linear_ space use: the algorithm space use grows together with respect to the input size `n`. That will happen if let's say for some reason the algorithm needs to allocate 'N' pointers (or other variables) when traversing a list.

**Source:** _stackoverflow.com_

#### Q10: What is an algorithm? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: What is complexity of this code snippet? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: What is the time complexity for "Hello, World" function? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: What is meant by "Constant Amortized Time" when talking about time complexity of an algorithm? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: Why do we use Big O instead of Big Theta (Θ)? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: Name some types of Big O complexity and corresponding algorithms ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: What is complexity of "Reading a Book"? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: Explain your understanding of "Space Complexity" with examples ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: What is the difference between Lower bound and Tight bound? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: What does it mean if an operation is <code><i>O</i>(<i>n!</i>)</code>? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q20: Provide an example of algorithm with time complexity of <code><i>O</i>(<i>c</i><sup>k</sup>)</code>? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q21: What are some algorithms which we use daily that has _`O(1)`_, _`O(n log n)`_ and _`O(log n)`_ complexities? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q22: What is the big O notation of this function? 
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=BinaryTree>Binary Tree</a> Interview Questions
#### Q1: Define Binary Tree ⭐
**Answer:**
A normal tree has no restrictions on the number of children each node can have. A **binary tree** is made of nodes, where each node contains a "left" pointer, a "right" pointer, and a data element. 

There are three different types of binary trees:

* **Full binary tree**: Every node other than leaf nodes has 2 child nodes.
* **Complete binary tree**: All levels are filled except possibly the last one, and all nodes are filled in as far left as possible.
* **Perfect binary tree**: All nodes have two children and all leaves are at the same level.



![](https://study.com/cimages/multimages/16/0e0646ba-30e5-40d9-b45c-a138f038f05b_full_complete_perfect.png)



**Source:** _study.com_

#### Q2: What is Binary Search Tree? ⭐⭐
**Answer:**
**Binary search tree** is a data structure that quickly allows to maintain a _sorted list_ of numbers.

* It is called a _binary tree_ because each tree node has maximum of two children.
* It is called a _search tree_ because it can be used to search for the presence of a number in `O(log n)` time.

The properties that separates a binary search tree from a regular binary tree are:

* All nodes of left subtree are less than root node
* All nodes of right subtree are more than root node
* Both subtrees of each node are also BSTs i.e. they have the above two properties


![](https://cdn.programiz.com/sites/tutorial2program/files/bst-vs-not-bst.jpg)


**Source:** _www.programiz.com_

#### Q3: Explain the difference between Binary Tree and Binary Search Tree with an example? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q4: Why do we want to use Binary Search Tree? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q5: What is AVL Tree? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: What are advantages and disadvantages of BST? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: What is Balanced Tree and why is that important? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: Convert a Binary Tree to a Doubly Linked List ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: What is the difference between Heap and Red-Black Tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: Explain how to balance AVL Tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: How does inserting or deleting nodes affect a Red-Black tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12:  Explain what the main differences between red-black (RB) trees and AVL trees ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: What is Red-Black tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: Build a Binary Expression Tree for this expression ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: What is the time complexity for insert into Red-Black Tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: Is there any reason anyone should use BSTs instead of AVLs in the first place? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: What are main advantages of Tries over Binary Search Trees (BSTs)? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: What's the main reason for choosing Red Black (RB) trees instead of AVL trees? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: How is an AVL tree different from a B-tree? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=BitManipulation>Bit Manipulation</a> Interview Questions
#### Q1: What is Bit? ⭐
**Answer:**
**Bit** stands for **Binary Digit** and is the _smallest unit of data_ in a computer. Binary digits can only be `0` or `1` because they are a `2- base` number. This means that if we want to represent the number `5` in binary we would have to write `0101`.



![](https://miro.medium.com/max/1400/1*8iteNc-7zXzaEfE5vLVkXQ.png)
<br/>

An integer variable usually have a 32 bits limit, which means it consists of 32 bits with its range of 2³² (2 derived from the state of bits — 0 or 1 which is 2 possibilities).

#### Q2: What would the number 22 look like as a Byte? ⭐⭐
**Answer:**
A byte is made up of 8 bits and the highest value of a byte is 255, which would mean every bit is set.

Now:
<table>
    <tbody>
    <tr> 
    <td colspan="11"> 
    1 
    Byte ( 8 bits )
    </td>
    </tr>
    <tr> 
    <td>Place 
    Value</td>
    <td> 
    128
    </td>
    <td> 
    64
    </td>
    <td> 
    32
    </td>
    <td> 
    16
    </td>
    <td> 
    8
    </td>
    <td> 
    4
    </td>
    <td> 
    2
    </td>
    <td> 
    1
    </td>
    <td></td>
    <td></td>
    </tr>
    <tr> 
    <td>&nbsp;</td>
    <td> 
    <div align="center">0
    </td>
    <td> 
    <div align="center">0
    </td>
    <td> 
    <div align="center">0
    </td>
    <td> 
    <div align="center">1
    </td>
    <td> 
    <div align="center">0
    </td>
    <td> 
    <div align="center">1
    </td>
    <td> 
    <div align="center">1
    </td>
    <td> 
    <div align="center">0
    </td>
    <td>
    <div align="center">=
    </td>
    <td>
    <div align="center">22
    </td>
    </tr>
    </tbody>
</table>
<br/>

Lets take it right to left and add up all those values together:

128 * `0` + 64 * `0` + 32 * `0` + 16 * `1` + 8 * `0` + 4 * `1` + 2 * `1` + 1 * `0`   = 22  



**Source:** _github.com_

#### Q3: What is a Byte? ⭐⭐
**Answer:**
A **byte** is made up of 8 bits and the highest value of a byte is 255, which would mean every bit is set. We will look at why a byte's maximum value is 255 in just a second.

So if all bits are set and the value = 255 my byte would look like this:

<table>
    <tbody>
        <tr> 
            <td colspan="11"> 
                1 Byte ( 8 bits )
            </td>
        </tr>
    <tr> 
        <td>
            Place Value
        </td>
        <td> 
          128
        </td>
        <td> 
          64
        </td>
        <td> 
          32
        </td>
        <td> 
          16
        </td>
        <td> 
          8
        </td>
        <td> 
          4
        </td>
        <td> 
          2
        </td>
        <td> 
          1
        </td>
        <td></td>
        <td></td>
    </tr>
    <tr> 
        <td>&nbsp;</td>
        <td> 
          <div align="center">1
        </td>
        <td> 
          <div align="center">1
        </td>
        <td> 
          <div align="center">1
        </td>
        <td> 
          <div align="center">1
        </td>
        <td> 
          <div align="center">1
        </td>
        <td> 
          <div align="center">1
        </td>
        <td> 
          <div align="center">1
        </td>
        <td> 
          <div align="center">1
        </td>
        <td>
          <div align="center">=
        </td>
        <td>255</td>
    </tr>
    </tbody>
</table>
<br/>
Lets take it right to left and add up all those values together
1 + 2 + 4 + 8 + 16 + 32 + 64 + 128 = 255

**Source:** _github.com_

#### Q4: Name some bitwise operations you know ⭐⭐
**Answer:**
* **NOT ( ~ )**: Bitwise NOT is an unary operator that flips the bits of the number i.e., if the ith bit is 0, it will change it to 1 and vice versa. 
* **AND ( & )**: Bitwise AND is a binary operator that operates on two equal-length bit patterns. If both bits in the compared position of the bit patterns are 1, the bit in the resulting bit pattern is 1, otherwise 0.
* **OR ( | )**: Bitwise OR is also a binary operator that operates on two equal-length bit patterns, similar to bitwise AND. If both bits in the compared position of the bit patterns are 0, the bit in the resulting bit pattern is 0, otherwise 1.
* **XOR ( ^ )**: Bitwise XOR also takes two equal-length bit patterns. If both bits in the compared position of the bit patterns are 0 or 1, the bit in the resulting bit pattern is 0, otherwise 1.

```js
AND|0 1      OR|0 1
---+----    ---+----
  0|0 0       0|0 1
  1|0 1       1|1 1

XOR|0 1     NOT|0 1
---+----    ---+---
  0|0 1        |1 0
  1|1 0
```

* **Left Shift ( << )**: Left shift operator is a binary operator which shift the some number of bits, in the given bit pattern, to the left and append 0 at the end.

* **Signed Right Shift ( >> )**: Right shift operator is a binary operator which shift the some number of bits, in the given bit pattern, to the right, preserving the sign (which is the first bit)

* **Zero Fill Right Shift ( >>> )**: Shifts right by pushing zeros in from the left, filling in the left bits with 0s

**Source:** _www.hackerearth.com_

#### Q5: Explain what is Bitwise operation? ⭐⭐
**Answer:**
**Bitwise operators** are used for _manipulating a data at the bit level_, also called as bit level programming. It is a fast and simple action, directly supported by the processor, and is used to manipulate values for comparisons and calculations.

On simple low-cost processors, typically, bitwise operations are substantially faster than division, several times faster than multiplication, and sometimes significantly faster than addition.

**Source:** _en.wikipedia.org_

#### Q6: Flip all bits in an integer ⭐⭐
**Details:**
I have to flip all bits in a binary representation of an integer. Given:

```js
10101
```

The output should be

```js
01010
```

What is the bitwise operator to accomplish this when used with an integer?

**Answer:**
Simply use the bitwise **not** operator `~`.

```js
int flipBits(int n) {
    return ~n;
}
```

**Source:** _stackoverflow.com_

#### Q7: What are some real world use cases of the bitwise operators? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: Explain how XOR (^) bit operator works ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: What are the advantages of using bitwise operations? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: What is difference between `>>` and `>>>` operators? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: What is Bit Masking? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Flip k least significant bits in an integer ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Blockchain>Blockchain</a> Interview Questions
#### Q1: What is blockchain? ⭐
**Answer:**
**Blockchain** is a secure distributed ledger (data structure or database) that maintains a continuously growing list of ordered records, called “blocks”,  that are linked using cryptography. Each block contains a cryptographic hash of the previous block, a timestamp, and transaction data.

By design, a blockchain is resistant to modification of the data. It is "an open, distributed ledger that can record transactions between two parties efficiently and in a verifiable and permanent way".

Once recorded, the data in any given block cannot be altered retroactively without alteration of all subsequent blocks, which requires consensus of the network majority. 

**Source:** _en.wikipedia.org_

#### Q2: What is blockchain transaction? ⭐⭐
**Answer:**
**Transactions** are the things that give a blockchain purpose. They are the smallest building blocks of a blockchain system. Transactions generally consist of:
* a recipient address, 
* a sender address, 
* and a value. 

This is not too different from a standard transaction that you would find on a credit card statement.

A transaction _changes the state_ of the agreed-correct blockchain. A blockchain is a shared, decentralized, distributed state machine. This means that all nodes (users of the blockchain system) independently hold their own copy of the blockchain, and the current known "state" is calculated by processing each transaction in order as it appears in the blockchain.

**Source:** _pluralsight.com_

#### Q3: Explain the common structure of blockchains ⭐⭐
**Answer:**
Blockchains are composed of three core parts:
* **Block**: A list of transactions recorded into a ledger over a given period. The size, period, and triggering event for blocks is different for every blockchain.
* **Chain**: A hash that links one block to another, mathematically “chaining” them together. 
* **Network**: The network is composed of “full nodes.” Think of them as the computer running an algorithm that is securing the network. Each node contains a complete record of all the transactions that were ever recorded in that blockchain.

**Source:** _dummies.com_

#### Q4: What is the blockchain data structure? ⭐⭐
**Answer:**
Basically **the blockchain data structure** is explained as a back-linked record of blocks of transactions, which is ordered. It can be saved as a file or in a plain database. Each block can be recognized by a hash, created utilizing the SHA256 cryptographic hash algorithm on the header of the block. Each block mentions a former block, also identified as the parent block, in the “previous block hash” field, in the block header.

![](https://vitalflux.com/wp-content/uploads/2018/06/Blockchain-represented-as-Linked-List-Data-Structure.png)


**Source:** _cryptoticker.io_

#### Q5: What is the purpose of a blockchain node? ⭐⭐
**Answer:**
A blockchain exists out of blocks of data. These blocks of data are stored on nodes (compare it to small servers). **Nodes** can be any kind of device (mostly computers, laptops or even bigger servers). Nodes form the infrastructure of a blockchain. 

All nodes on a blockchain are connected to each other and they constantly exchange the latest blockchain data with each other so all nodes stay up to date. They store, spread and preserve the blockchain data, so theoretically a blockchain exists on nodes. 

A **full node** is basically a device (like a computer) that contains a full copy of the transaction history of the blockchain.

**Source:** _lisk.io_

#### Q6: What is the Genesis Block? ⭐⭐
**Answer:**
The **first block in any blockchain **is termed the **genesis block**. If you start at any block and follow the chain backwards chronologically, you will arrive at the genesis block. The genesis block is statically encoded within the client software, that it cannot be changed. Every node can identify the genesis block’s hash and structure, the fixed time of creation, and the single transactions within. Thus every node has a secure “root” from which is possible to build a trusted blockchain on.

**Source:** _linkedin.com_

#### Q7: What is proof-of-work? ⭐⭐
**Answer:**
A **proof of work** is a piece of data which is difficult (costly, time-consuming) to produce but easy for others to verify and which satisfies certain requirements. Producing a proof of work can be a random process with low probability so that a lot of trial and error is required on average before a valid proof of work is generated. Difficulty is a measure of how difficult it is to find a hash below a given target.

**Source:** _en.bitcoin.it_

#### Q8: Why does Blockchain need coins or tokens? ⭐⭐
**Answer:**
_Tokens/Coins are used as a medium of exchange between the states_. They are digital assets built in to perform a specific function within a blockchain.

When someone does a transaction, there is a _change of state_, and coins are moved from one address to another address. Apart from that, transactions contain some additional data; this data can be mutated through the change of state. For this reason, blockchains need coins or tokens to incentivize the participants to join their networks.

**Source:** _mindmajix.com_

#### Q9: What is deterministic behavior? ⭐⭐
**Answer:**
If A + B = C, then no matter what the circumstances, A+B will always be equal to C. That is called deterministic behavior.

Hash functions are deterministic, meaning A’s hash will always be H(A).

**Source:** _blockgeeks.com_

#### Q10: What is block data structure in blockchain? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: Why is the blockchain immutable? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Explain why there is a fixed supply of bitcoins? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: What is mining difficulty? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: What is a hashing function? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: What are some advantages of using Merke Trees? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: How Are Blockchain And Distributed Ledger Different? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: What is Merkle Trees? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: Explain what do nodes do?  ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: How do verifiers check if a block is valid? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q20: What is DApp or Decentralised Application? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q21: What are the major elements of the blockchain ecosystem? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q22: Explain why a blockchain needs tokens to operate ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q23: What are the core components of blockchain architecture? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q24: What is RSA algorithm? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q25: What is a trapdoor function, and why is it needed in blockchain development? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q26: What is a smart contract? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q27: What's the difference between distributed hashtable technology and the bitcoin blockchain? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q28: What determines the mining difficulty? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q29: What is a 51% attack? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q30: What is the difference between PoW and PoS? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q31: What Is a Blockchain Consensus Algorithm? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q32: How is hard fork different from the soft fork in blockchain? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q33: What Is a Proof of Stake? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q34: What is a stealth address? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q35: Name some widespread platforms for developing blockchain applications ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q36: Explain what is target hash? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q37: What is nonce? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q38: What is off-chain transaction? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q39: Why is Git not considered a “block chain”? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q40: What can an attacker with 51% of hash power do? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q41: What are miners really solving? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q42: Is it possible to brute force bitcoin address creation in order to steal money? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=BrainTeasers>Brain Teasers</a> Interview Questions
#### Q1: How do you swap two numbers without using the third variable? ⭐⭐
**Answer:**
You can swap two numbers without using a temporary or third variable if you can _store the sum of numbers in one number and then minus the sum with other number_, something like:

```js
a = 3;
b = 5;

a = a + b; //8
b = a — b; // 3
a = a — b; //5
```

now you have `a = 5` and `b = 3`, so numbers are swapped without using a third or temp variable.

**Source:** _javarevisited.blogspot.com_

#### Q2: Write a function that guarantees to never return the same value twice ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q3: How can I pair socks from a pile efficiently? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q4: How to check for braces balance in a really large (1T) file in parallel? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Divide&Conquer>Divide & Conquer</a> Interview Questions
#### Q1: Explain how Merge Sort works ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q2: What is the difference between Divide and Conquer and Dynamic Programming Algorithms? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q3: Convert a Binary Tree to a Doubly Linked List ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q4: Explain how QuickSort works ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q5: Compare Greedy vs Divide & Conquer vs Dynamic Programming Algorithms ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: Explain what is Fibonacci Search technique? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=DynamicProgramming>Dynamic Programming</a> Interview Questions
#### Q1: What is Dynamic Programming? ⭐
**Answer:**
**Dynamic programming** is all about ordering your computations in a way that avoids recalculating duplicate work. More specifically, Dynamic Programming is a technique used to avoid computing multiple times the same _subproblem_ in a recursive algorithm. DP algorithms could be implemented with recursion, but they don't have to be.

With dynamic programming, you store your results in some sort of table generally. When you need the answer to a problem, you reference the table and see if you already know what it is. If not, you use the data in your table to give yourself a stepping stone towards the answer.

There are two approaches to apply Dynamic Programming:
* The **top-down or memoization**. When the recursion does a lot of unecessary calculation, an easy way to solve this is to cache the results and to check before executing the call if the result is already in the cache.
* The **bottom-up or tabulation approach**. A better way to do this is to get rid of the recursion all-together by evaluating the results in the right order and building the array as we iterate. The partial results are available when needed if the iteration is done in the right order.

```js
TOP of the tree
fib(4)
 fib(3)...................... + fib(2)
  fib(2)......... + fib(1)       fib(1)........... + fib(0)
   fib(1) + fib(0)   fib(1)       fib(1)              fib(0)
    fib(1)   fib(0)
BOTTOM of the tree
```


**Source:** _stackoverflow.com_

#### Q2: How Dynamic Programming is different from Recursion and Memoization? ⭐⭐
**Answer:**
* **Memoization** is when you store previous results of a function call (a real function always returns the same thing, given the same inputs). It doesn't make a difference for algorithmic complexity before the results are stored.
* **Recursion** is the method of a function calling itself, usually with a smaller dataset. Since most recursive functions can be converted to similar iterative functions, this doesn't make a difference for algorithmic complexity either.
* **Dynamic programming** is the process of solving easier-to-solve sub-problems and building up the answer from that. Most DP algorithms will be in the running times between a Greedy algorithm (if one exists) and an exponential (enumerate all possibilities and find the best one) algorithm.
  * DP algorithms could be implemented with recursion, but they don't have to be.
  * DP algorithms can't be sped up by memoization, since each sub-problem is only ever solved (or the "solve" function called) once.

**Source:** _stackoverflow.com_

#### Q3: What are some characteristics of Dynamic Programming?  ⭐⭐
**Answer:**
The key idea of DP is to save answers of overlapping smaller sub-problems to avoid recomputation. For that:
* An instance is solved using the solutions for smaller instances.
* The solutions for a smaller instance might be needed multiple times, so store their results in a table.
* Thus each smaller instance is solved only once.
* Additional space is used to save time.

**Source:** _stackoverflow.com_

#### Q4: What are pros and cons of Memoization or Top-Down approach? ⭐⭐
**Answer:**
**Pros**: 
 * Memoization is very easy to code (you can generally* write a "memoizer" annotation or wrapper function that automatically does it for you), and should be your first line of approach. It feels more natural. You can take a recursive function and memoize it by a mechanical process (first lookup answer in cache and return it if possible, otherwise compute it recursively and then before returning, you save the calculation in the cache for future use), whereas doing bottom up dynamic programming requires you to encode an order in which solutions are calculated.
 * Top-down only solves sub-problems used by your solution whereas bottom-up might waste time on redundant sub-problems.

**Cons**: 
 * With memoization, if the tree is very deep (e.g. <code>fib(10<sup>6</sup>)</code>), you will run out of stack space, because each delayed computation must be put on the stack, and you will have <code>10<sup>6</sup></code> of them.

**Source:** _stackoverflow.com_

#### Q5: Provide an example of Dynamic Program but without Recursion ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: What are some pros and cons of Tabulation or Bottom-Up approach? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: What should you consider when choosing between Top-Down vs Bottom-Up solutions for the same problem? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: LIS: Find length of the longest increasing subsequence (LIS) in the array. Solve using DP. ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: What is the difference between Divide and Conquer and Dynamic Programming Algorithms? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: How to use Memoization for N-th Fibonacci number?  ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: Compare Greedy vs Divide & Conquer vs Dynamic Programming Algorithms ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Is Dijkstra's algorithm a Greedy or Dynamic Programming algorithm? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=FibonacciSeries>Fibonacci Series</a> Interview Questions
#### Q1: What is Fibonacci Sequence of numbers? ⭐
**Answer:**
The **Fibonacci Sequence** is the series of numbers:

```js
0, 1, 1, 2, 3, 5, 8, 13, 21, 34, ...
```
Fibonacci sequence characterized by the fact that every number after the **first two is the sum of the two preceding ones**:
```js
Fibonacci(0) = 0, 
Fibonacci(1) = 1,
Fibonacci(n) = Fibonacci(n-1) + Fibonacci(n-2)  
```

**Fibonacci sequence**, appears a lot in nature. Patterns such as spirals of shells, curve of waves, seed heads, pinecones, and branches of trees can all be described using this mathematical sequence. The fact that things as large as spirals of galaxies, and as small as DNA molecules follow the Golden Ratio rule suggests that Fibonacci sequence is one of the most fundamental characteristics of the Universe.

![](https://www.mathsisfun.com/numbers/images/fibonacci-spiral.svg)


**Source:** _www.mathsisfun.com_

#### Q2: What is Golden Ratio? ⭐⭐
**Answer:**
When we take any two successive (one after the other) Fibonacci Numbers, their ratio is very close to the Golden Ratio `φ` which is approximately `1.618034...`. In fact, the bigger the pair of Fibonacci Numbers, the closer the approximation. Let us try a few:

```js
3/2 = 1.5
5/3 = 1.666666666...
...
233/377 = 1.618055556...
```
This also works when we pick two random whole numbers to begin the sequence, such as 192 and 16 (we get the sequence 192, 16, 208, 224, 432, 656, 1088, 1744, 2832, 4576, 7408, 11984, 19392, 31376, ...):
```js
16/192 = 0.08333333...
208/16 = 13
...
11984/7408 = 1.61771058...
19392/11984 = 1.61815754...
```

**Source:** _www.mathsisfun.com_

#### Q3: Return the N-th value of the Fibonacci sequence. Solve in _`O(n)`_ time ⭐⭐
**Answer:**
The easiest solution that comes to mind here is iteration: 

```js
function fib(n){
  let arr = [0, 1];
  for (let i = 2; i < n + 1; i++){
    arr.push(arr[i - 2] + arr[i -1])
  }
 return arr[n]
}
```
And output:
```
fib(4)
=> 3
```


Notice that two first numbers can not really be effectively generated by a for loop, because our loop will involve adding two numbers together, so instead of creating an empty array we assign our arr variable to `[0, 1]` that we know for a fact will always be there. After that we create a loop that starts iterating from i = 2 and adds numbers to the array until the length of the array is equal to `n + 1`. Finally, we return the number at n index of array.

**Source:** _medium.com_

#### Q4: Return the N-th value of the Fibonacci sequence Recursively ⭐⭐
**Answer:**
Recursive solution looks pretty simple (see code).

Let’s look at the diagram that will help you understand what’s going on here with the rest of our code. Function fib is called with argument 5:

![](https://miro.medium.com/max/1400/1*LNBBacuaBFOVZXUV6VgEEg.png)

Basically our **fib** function will continue to recursively call itself creating more and more branches of the tree until it hits the base case, from which it will start summing up each branch’s return values bottom up, until it finally sums them all up and returns an integer equal to 5.

**Source:** _medium.com_

#### Q5: Get the N-th Fibonacci number with _`O(n)`_ time and _`O(1)`_ space complexity ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: Display startNumber to endNumber only from Fibonacci Sequence ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: How to use Memoization for N-th Fibonacci number?  ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: Get Fibonacci Number in <code><i>O</i>(<i>log n</i>)</code> time using Matrix Exponentiation ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: Test if a Number belongs to the Fibonacci Series ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: Calculate n-th Fibonacci number using Tail Recursion ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: Binet's formula: How to calculate Fibonacci numbers without Recursion or Iteration?  ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Explain what is Fibonacci Search technique? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: Can a Fibonacci function be written to execute in _`O(1)`_ time? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: Generating Fibonacci Sequence using ES6 generator functions ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=GraphTheory>Graph Theory</a> Interview Questions
#### Q1: What is a Graph? ⭐
**Answer:**
A **graph** is a common data structure that consists of a finite set of **nodes** (or **vertices**) and a set of **edges** connecting them. A pair `(x,y)` is referred to as an edge, which communicates that the **x vertex** connects to the **y vertex**.

Graphs are used to solve real-life problems that involve representation of the problem space as a **network**. Examples of networks include telephone networks, circuit networks, social networks (like LinkedIn, Facebook etc.).



![](https://miro.medium.com/max/1640/1*4s5Z7gVwVqmKcslgiamRyw.png)


**Source:** _www.educative.io_

#### Q2: What's the difference between the data structure Tree and Graph? ⭐⭐
**Answer:**
**Graph:**
* Consists of a set of vertices (or nodes) and a set of edges connecting some or all of them
* Any edge can connect any two vertices that aren't already connected by an identical edge (in the same direction, in the case of a directed graph)
* Doesn't have to be connected (the edges don't have to connect all vertices together): a single graph can consist of a few disconnected sets of vertices
* Could be directed or undirected (which would apply to all edges in the graph)

**Tree:**
* A type of graph (fit with in the category of Directed Acyclic Graphs (or a DAG))
* Vertices are more commonly called "nodes"
* Edges are directed and represent an "is child of" (or "is parent of") relationship
* Each node (except the root node) has exactly one parent (and zero or more children)
* Has exactly one "root" node (if the tree has at least one node), which is a node without a parent
* Has to be connected
* Is acyclic, meaning it has no cycles: "a cycle is a path [AKA sequence] of edges and vertices wherein a vertex is reachable from itself"
* Trees aren't a recursive data structure



![](https://miro.medium.com/max/2262/1*-yHATwTlY2hwceJ93-D-cw.jpeg)


**Source:** _stackoverflow.com_

#### Q3: List some ways of representing Graphs ⭐⭐
**Answer:**
* **Edge Lists**. We have an array of two vertex numbers, or an array of objects containing the vertex numbers of the vertices that the edges are incident on (plus weight). Edge lists are simple, but if we want to find whether the graph contains a particular edge, we have to search through the edge list. If the edges appear in the edge list in no particular order, that's a linear search through `E` edges.
```js
[ [0,1], [0,6], [0,8], [1,4], [1,6], [1,9], [2,4], [2,6], [3,4], [3,5], [3,8], [4,5], [4,9], [7,8], [7,9] ]
```
* **Adjacency Matrices.** With an adjacency matrix, we can find out whether an edge is present in constant time, by just looking up the corresponding entry in the matrix - we can query whether edge `(i, j)` is in the graph by looking at `graph[i][j]` value. For a sparse graph, the adjacency matrix is mostly `0s`, and we use lots of space to represent only a few edges. For an undirected graph, the adjacency matrix is _symmetric_.
```js
[ [0, 1, 0, 0, 0, 0, 1, 0, 1, 0],
  [1, 0, 0, 0, 1, 0, 1, 0, 0, 1],
  [0, 0, 0, 0, 1, 0, 1, 0, 0, 0],
  [0, 0, 0, 0, 1, 1, 0, 0, 1, 0],
  [0, 1, 1, 1, 0, 1, 0, 0, 0, 1],
  [0, 0, 0, 1, 1, 0, 0, 0, 0, 0],
  [1, 1, 1, 0, 0, 0, 0, 0, 0, 0],
  [0, 0, 0, 0, 0, 0, 0, 0, 1, 1],
  [1, 0, 0, 1, 0, 0, 0, 1, 0, 0],
  [0, 1, 0, 0, 1, 0, 0, 1, 0, 0] ]
```
* **Adjacency Lists**. For each vertex `i`, store an array of the vertices adjacent to it (or array of _tuples_ for weighted graph). To find out whether an edge `(i,j)` is present in the graph, we go to `i's` adjacency list in constant time and then look for `j` in `i's` adjacency list.
```js
[ [1, 6, 8],   // 0
  [0, 4, 6, 9],  // 1
  [4, 6],        // 2
  [4, 5, 8],
  [1, 2, 3, 5, 9],
  [3, 4],
  [0, 1, 2],
  [8, 9],
  [0, 3, 7],
  [1, 4, 7] ]    // N
```


![](https://www.educative.io/api/edpresso/shot/6738347923865600/image/4587527119831040)


**Source:** _www.khanacademy.org_

#### Q4: Explain what is DFS (Depth First Search) algorithm for a Graph and how does it work? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q5: Explain what is `A*` Search? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: What is difference between BFS and Dijkstra's algorithms when looking for shortest path? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: Compare Adjacency Lists or Adjacency Matrices for Graphs representation ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: Provide some practical examples of using Depth-First Search (DFS) vs Breadth-First Search (BFS)? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: What are some applications of Graphs? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: Explain the BSF (Breadth First Search) traversing method ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: Name some common types and categories of Graphs ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Why is the complexity of DFS _`O(V+E)`_? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: What are key differences between BFS and DFS? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: What is Bipartite Graph? How to detect one? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: How do we know whether we need to use BSF or DSF algorithm? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: Why does a Breadth First Search (BFS) use more memory than Depth First Search (DFS)? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: Explain what is heuristic cost function in `A*` Search and how to calculate one? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: What's the difference between best-first search and `A*` Search? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: Illustrate the difference in peak memory consumption between DFS and BFS ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=GreedyAlgorithms>Greedy Algorithms</a> Interview Questions
#### Q1: What is a Greedy Algorithm? ⭐
**Answer:**
We call algorithms *greedy* when they utilise the greedy property. The greedy property is:

> At that exact moment in time, what is the optimal choice to make?

Greedy algorithms are _greedy_. They do not look into the future to decide the global optimal solution. They are only concerned with the optimal solution _locally_. This means that **the overall optimal solution may differ from the solution the greedy algorithm chooses.**

They never look backwards at what they've done to see if they could optimise globally. This is the main difference between Greedy Algorithms and Dynamic Programming.

**Source:** _skerritt.blog_

#### Q2: What Are Greedy Algorithms Used For? ⭐⭐
**Answer:**
Greedy algorithms are quick. A lot faster than the two other alternatives (Divide & Conquer, and Dynamic Programming). They're used because they're fast. Sometimes, Greedy algorithms give the global optimal solution every time. Some of these algorithms are:

* Dijkstra's Algorithm
* Kruskal's algorithm
* Prim's algorithm
* Huffman trees

These algorithms are Greedy, and their Greedy solution gives the optimal solution.

#### Q3: What is the difference between Dynamic Programming and Greedy Algorithms? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q4: Compare Greedy vs Divide & Conquer vs Dynamic Programming Algorithms ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q5: Is Dijkstra's algorithm a Greedy or Dynamic Programming algorithm? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: What's the difference between Greedy and Heuristic algorithm? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: Are there any proof to decide if Greedy approach will produce the best solution? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=HashTables>Hash Tables</a> Interview Questions
#### Q1: What is Hash Table? ⭐
**Answer:**
A **hash table** (hash map) is a data structure that implements an **associative** array abstract data type, a **structure** that can **map keys to values**. Hash tables implement an associative array, which is indexed by arbitrary objects (keys). A hash table uses a **hash function** to compute an **index**, also called a **hash value**, into an **array of buckets** or slots, from which the desired **value** can be found.


![](https://i.stack.imgur.com/0yjYd.png)


**Source:** _en.wikipedia.org_

#### Q2: What is Hashing? ⭐⭐
**Answer:**
**Hashing** is the practice of using **an algorithm (or hash function)** to map data of _any_ size to a _fixed_ length. This is called a hash value (or sometimes hash code or hash sums or even a hash digest if you’re feeling fancy). In hashing, keys are converted into _hash values_ or _indexes_ by using **hash functions**. Hashing is a one-way function.

**Source:** _www.thesslstore.com_

#### Q3: Explain what is Hash Value? ⭐⭐
**Answer:**
A **Hash Value** (also called as Hashes or Checksum) is a string value (of specific length), which is the result of calculation of a Hashing Algorithm. Hash Values have different uses:

1. Indexing for Hash Tables
2. Determine the Integrity of any Data (which can be a file, folder, email, attachments, downloads etc).

**Source:** _www.omnisecu.com_

#### Q4: What is the space complexity of a Hash Table? ⭐⭐
**Answer:**
The space complexity of a datastructure indicates how much space it occupies in relation to the amount of elements it holds. For example a space complexity of `O(1)` would mean that the datastructure alway consumes constant space no matter how many elements you put in there. `O(n)` would mean that the space consumption grows linearly with the amount of elements in it.

A **hashtable** typically has a space complexity of `O(n)`.

**Source:** _stackoverflow.com_

#### Q5: Define what is a Hash Function? ⭐⭐
**Answer:**
A **hash function** is any function that can be used to map data of arbitrary size to fixed-size values. The values returned by a hash function are called _hash values_, hash codes, digests, or simply hashes. The values are used to index a fixed-size table called a hash table. Use of a hash function to index a hash table is called _hashing_ or _scatter storage addressing_.

Mathematically speaking, a **hash function** is usually defined as a mapping from the universe of elements you want to store in the hash table to the range `{0, 1, 2, .., numBuckets - 1}`. 

Some properties of Hash Functions are:

* Very fast to compute (nearly constant)
* One way; can not be reversed
* Output does not reveal information on input
* Hard to find collisions (different data with same hash)
* Implementation is based on parity-preserving bit operations (XOR and ADD), multiply, or divide. 

**Source:** _en.wikipedia.org_

#### Q6: Detect if a List is Cyclic using Hash Table ⭐⭐
**Answer:**
To detect if a list is cyclic, we can check whether a node had been visited before. A natural way is to use a hash table.

**Algorithm**

We go through each node one by one and record each node's reference (or memory address) in a hash table. If the current node is `null`, we have reached the end of the list and it must not be cyclic. If current node’s reference is in the hash table, then return true.

**Source:** _leetcode.com_

#### Q7: What is the significance of load factor of a Hash Table? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: What does "bucket entries" mean in the context of a hashtable? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: What is complexity of Hash Table? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: What is Hash Collision? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: Explain in simple terms how Hash Tables are implemented? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Remove duplicates from an unsorted Linked List ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: Find similar elements from two Linked Lists and return the result as a Linked List ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: Explain some technics to handle collision in Hash Tables ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: How can I pair socks from a pile efficiently? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: Compare lookup operation in Trie vs Hash Table ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: What are some main advantages of Tries over Hash Tables ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: How To Choose Between a Hash Table and a Trie (Prefix Tree)? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=HeapsandMaps>Heaps and Maps</a> Interview Questions
#### Q1: What is Heap? ⭐
**Answer:**
A **Heap** is a special Tree-based data structure which is an almost complete tree that satisfies the heap property:

* in a **max heap**, for any given node C, if P is a parent node of C, then the key (the value) of P is greater than or equal to the key of C. 
* In a **min heap**, the key of P is less than or equal to the key of C. The node at the "top" of the heap (with no parents) is called the root node.


A common implementation of a heap is the binary heap, in which the tree is a **binary tree.**


![](https://www.techiedelight.com/wp-content/uploads/2016/11/Min-Max-Heap.png)


**Source:** _www.geeksforgeeks.org_

#### Q2: What is Priority Queue? ⭐
**Answer:**
A **priority queue** is a data structure that stores **priorities** (comparable values) and perhaps associated information.  A **priority queue** is different from a "normal" queue, because instead of being a "first-in-first-out" data structure, values come out in order by **priority**. Think of a priority queue as a kind of bag that holds priorities. You can put one in, and you can take out the current highest priority.

![](https://cdn.programiz.com/sites/tutorial2program/files/Introduction.png)


**Source:** _pages.cs.wisc.edu_

#### Q3: How is Binary Heap usually implemented? ⭐⭐
**Answer:**
A **binary heaps** are commonly implemented with an **array**. Any binary tree can be stored in an array, but because a binary heap is always a _complete_ binary tree, it can be stored compactly. No space is required for pointers; instead, the parent and children of each node can be found by arithmetic on array indices:

* The root element is `0`
* Left child : `(2*i)+1`
* Right child : `(2*i)+2`
* Parent child : `(i-1)/2`


![](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c4/Binary_Heap_with_Array_Implementation.JPG/800px-Binary_Heap_with_Array_Implementation.JPG)


**Source:** _www.geeksforgeeks.org_

#### Q4: Insert item into the Heap. Explain your actions. ⭐⭐
**Details:**
Suppose I have a Heap Like the following:

```
     77
    /  \
   /    \
  50    60
 / \    / \
22 30  44 55
```
Now, I want to insert another item 55 into this Heap. How to do this?

**Answer:**
A **binary heap** is defined as a binary tree with two additional constraints:

* **Shape property**: a binary heap is a complete binary tree; that is, all levels of the tree, except possibly the last one (deepest) are fully filled, and, if the last level of the tree is not complete, the nodes of that level are filled from left to right.
* **Heap property**: the key stored in each node is either greater than or equal to (≥) or less than or equal to (≤) the keys in the node's children, according to some total order.

We start adding child from the most left node and if the parent is lower than the newly added child than we replace them. And like so will go on until the child got the parent having value greater than it.

Your initial tree is:

```js
     77
    /  \
   /    \
  50    60
 / \    / \
22 30  44 55
```
Now adding 55 according to the rule on most left side:
```
     77
    /  \
   /    \
  50    60
 / \    / \
22 30  44 55
/
55
```
But you see 22 is lower than 55 so replaced it:
```
       77
      /  \
     /    \
    50    60
   / \    / \
  55 30  44 55
 /
22 
```
Now 55 has become the child of 50 which is still lower than 55 so replace them too:
```
       77
      /  \
     /    \
    55    60
   / \    / \
  50 30  44 55
 /
22
```
Now it cant be sorted more because 77 is greater than 55.

**Source:** _stackoverflow.com_

#### Q5: What is Binary Heap? ⭐⭐
**Answer:**
A **Binary Heap** is a _Binary Tree_ with following properties:

* It’s a _complete_ tree (all levels are completely filled except possibly the last level and the last level has all keys as left as possible). This property of Binary Heap makes them suitable to be stored in an array.
* A Binary Heap is either **Min Heap** or **Max Heap**. In a Min Binary Heap, the key at root must be minimum among all keys present in Binary Heap. The same property must be recursively true for all nodes in Binary Tree. Max Binary Heap is similar to MinHeap.

```js
            10                      10
         /      \               /       \  
       20        100          15         30  
      /                      /  \        /  \
    30                     40    50    100   40
```

**Source:** _www.geeksforgeeks.org_

#### Q6: What is the advantage of Heaps over Sorted Arrays? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: Explain how Heap Sort works ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: When would you want to use a Heap? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: Name some ways to implement Priority Queue ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: Compare Heaps vs Arrays to implement Priority Queue ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: What is the difference between Heap and Red-Black Tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Explain how to find 100 largest numbers out of an array of 1 billion numbers ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=LinkedLists>Linked Lists</a> Interview Questions
#### Q1: Define Linked List ⭐
**Answer:**
A **linked list** is a linear data structure where each element is a separate object. Each element (we will call it a **node**) of a list is comprising of two items - the **data** and a **reference (pointer)** to the next node. The last node has a reference to **null**. The entry point into a linked list is called the **head** of the list. It should be noted that _head is not a separate node,_ but the reference to the first node. If the list is empty then the head is a null reference.

**Source:** _www.cs.cmu.edu_

#### Q2: Name some advantages of Linked List ⭐
**Answer:**
There are some:
* Linked Lists are **Dynamic Data Structure** -  it can grow and shrink at runtime by allocating and deallocating memory. So there is no need to give initial size of linked list.
* Insertion and Deletion are **simple to implement** - Unlike array here we don’t have to shift elements after insertion or deletion of an element. In linked list we just have to update the address present in next pointer of a node.
* **Efficient Memory Allocation/No Memory Wastage** - In case of array there is lot of memory wastage, like if we declare an array of size 10 and store only 6 elements in it then space of 4 elements are wasted. There is no such problem in linked list as memory is allocated only when required.

**Source:** _www.thecrazyprogrammer.com_

#### Q3: What is a cycle/loop in the singly-linked list? ⭐⭐
**Answer:**
A **cycle/loop** occurs when a node’s next points _back_ to a _previous node_ in the list. The linked list is no longer linear with a beginning and end—instead, it cycles through a loop of nodes.


![](https://www.programcreek.com/wp-content/uploads/2012/12/linked-list-cycle-300x211.png)

**Source:** _www.interviewcake.com_

#### Q4: What are some types of Linked List? ⭐⭐
**Answer:**
* A **singly linked list**

![](https://www.cs.cmu.edu/~adamchik/15-121/lectures/Linked%20Lists/pix/linkedlist.bmp)
* A **doubly linked list** is a list that has two references, one to the next node and another to previous node.

![](https://www.cs.cmu.edu/~adamchik/15-121/lectures/Linked%20Lists/pix/doubly.bmp)
* A **multiply linked list** - each node contains two or more link fields, each field being used to connect the same set of data records in a different order of same set(e.g., by name, by department, by date of birth, etc.).
* A **circular linked list** - where last node of the list points back to the first node (or the head) of the list.

![](https://i2.wp.com/algorithms.tutorialhorizon.com/files/2016/03/Circular-Linked-List.png)


**Source:** _www.cs.cmu.edu_

#### Q5: What is time complexity of Linked List operations? ⭐⭐
**Answer:**
* A linked list can typically only be accessed via its head node. From there you can only traverse from node to node until you reach the node you seek. Thus **access is <code><i>O</i>(<i>n</i>)</code>**.
* Searching for a given value in a linked list similarly requires traversing all the elements until you find that value. Thus **search is <code><i>O</i>(<i>n</i>)</code>**.
* Inserting into a linked list requires re-pointing the previous node (the node before the insertion point) to the inserted node, and pointing the newly-inserted node to the next node. Thus **insertion is <code><i>O</i>(<i>1</i>)</code>**.
* Deleting from a linked list requires re-pointing the previous node (the node before the deleted node) to the next node (the node after the deleted node). Thus **deletion is <code><i>O</i>(<i>1</i>)</code>**.

**Source:** _github.com_

#### Q6: Name some disadvantages of Linked Lists? ⭐⭐
**Answer:**
Few disadvantages of linked lists are :

* They use more memory than arrays because of the storage used by their pointers.
* Difficulties arise in linked lists when it comes to reverse traversing. For instance, singly linked lists are cumbersome to navigate backwards and while doubly linked lists are somewhat easier to read, memory is wasted in allocating space for a back-pointer.
* Nodes in a linked list must be read in order from the beginning as linked lists are inherently sequential access.
* Random access has linear time.
* Nodes are stored incontiguously (no or poor cache locality), greatly increasing the time required to access individual elements within the list, especially with a CPU cache.
* If the link to list's node is accidentally destroyed then the chances of data loss after the destruction point is huge. Data recovery is not possible.
* Search is linear versus logarithmic for sorted arrays and binary search trees.
* Different amount of time is required to access each element.
* Not easy to sort the elements stored in the linear linked list.

**Source:** _www.quora.com_

#### Q7: How to reverse a singly Linked List using only two pointers? ⭐⭐
**Answer:**
Nothing faster than <code><i>O</i>(<i>n</i>)</code> can be done. You need to traverse the list and alter pointers on every node, so time will be proportional to the number of elements.

**Source:** _stackoverflow.com_

#### Q8: What is complexity of `push` and `pop` for a Stack implemented using a LinkedList? ⭐⭐
**Answer:**
<code><i>O</i>(<i>1</i>)</code>. Note, you don't have to insert at the end of the list. If you insert at the front of a (singly-linked) list, they are both `O(1)`.

Stack contains 1,2,3:

```py
[1]->[2]->[3]
```

Push 5:

```js
[5]->[1]->[2]->[3]
```

Pop:

```js
[1]->[2]->[3] // returning 5
```


**Source:** _stackoverflow.com_

#### Q9: Insert an item in a sorted Linked List maintaining order ⭐⭐
**Answer:**
The `add()` method below walks down the list until it finds the appropriate position. Then, it splices in the new node and updates the `start`, `prev`, and `curr` pointers where applicable.

Note that the reverse operation, namely _removing_ elements, doesn't need to change, because you are simply throwing things away which would not change any order in the list.


**Source:** _stackoverflow.com_

#### Q10: Convert a Singly Linked List to Circular Linked List ⭐⭐
**Answer:**
To convert a singly linked list to circular linked list, we will set next pointer of tail node to head pointer.

*   Create a copy of head pointer, let's say `temp`.
*   Using a loop, traverse linked list till tail node (last node) using temp pointer.
*   Now set the next pointer of tail node to head node. `temp\->next = head`

**Source:** _www.techcrashcourse.com_

#### Q11: Detect if a List is Cyclic using Hash Table ⭐⭐
**Answer:**
To detect if a list is cyclic, we can check whether a node had been visited before. A natural way is to use a hash table.

**Algorithm**

We go through each node one by one and record each node's reference (or memory address) in a hash table. If the current node is `null`, we have reached the end of the list and it must not be cyclic. If current node’s reference is in the hash table, then return true.

**Source:** _leetcode.com_

#### Q12: Under what circumstances are Linked Lists useful? ⭐⭐
**Answer:**
Linked lists are very useful when you need :
* to do a lot of insertions and removals, but not too much searching, on a list of arbitrary (unknown at compile\-time) length.
* splitting and joining (bidirectionally\-linked) lists is very efficient.
* You can also combine linked lists \- e.g. tree structures can be implemented as "vertical" linked lists (parent/child relationships) connecting together horizontal linked lists (siblings).

Using an array based list for these purposes has severe limitations:

*   Adding a new item means the array must be reallocated (or you must allocate more space than you need to allow for future growth and reduce the number of reallocations)
*   Removing items leaves wasted space or requires a reallocation
*   inserting items anywhere except the end involves (possibly reallocating and) copying lots of the data up one position

**Source:** _stackoverflow.com_

#### Q13: Convert a Single Linked List to a Double Linked List ⭐⭐
**Answer:**
A doubly linked list is simply a linked list where every element has both next and prev mebers, pointing at the elements before and after it, not just the one after it in a single linked list.

so to convert your list to a doubly linked list, just change your node to be:

```java
private class Node
{
    Picture data;
    Node pNext;
    Node pPrev;
};
```

and when iterating the list, on each new node add a reference to the previous node.

**Source:** _stackoverflow.com_

#### Q14: How to implement Linked List Using Stack? ⭐⭐
**Answer:**
You can simulate a linked list by using two stacks. One stack is the "list," and the other is used for temporary storage.

* To **add** an item at the head, simply push the item onto the stack. 
* To **remove** from the head, pop from the stack.
* To **insert** into the middle somewhere, pop items from the "list" stack and push them onto the temporary stack until you get to your insertion point. Push the new item onto the "list" stack, then pop from the temporary stack and push back onto the "list" stack. Deletion of an arbitrary node is similar.

This isn't terribly efficient, by the way, but it would in fact work.

**Source:** _stackoverflow.com_

#### Q15: Why does linked list delete and insert operation have complexity of _`O(1)`_? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: When to use a Linked List over an Array/Array List? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: Floyd's Cycle Detect Algorithm: Remove Cycle (Loop) from a Linked List ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: Compare Array based vs Linked List stack implementations ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: Floyd's Cycle Detect Algorithm: Explain how to find a starting node of a Cycle in a Linked List? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q20: Floyd's Cycle Detect Algorithm: How to detect a Cycle (or Loop) in a Linked List? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q21: When is a loop in a Linked List useful? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q22: Implement Double Linked List from Stack with min complexity ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q23:  Split the Linked List into `k` consecutive linked list "parts" ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q24: Remove duplicates from an unsorted Linked List ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q25: Sum two numbers represented as Linked Lists ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q26: Find similar elements from two Linked Lists and return the result as a Linked List ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q27: How to find _`Nth`_ element from the end of a singly Linked List? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q28: When should I use a List vs a LinkedList? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q29: Merge two sorted singly Linked Lists without creating new nodes ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q30: Convert a Binary Tree to a Doubly Linked List ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q31: How would you compare Dynamic Arrays with Linked Lists and vice versa?  ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q32: How to recursively reverse a Linked List? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q33: Why is Merge sort preferred over Quick sort for sorting Linked Lists? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q34: Find Merge (Intersection) Point of Two Linked Lists ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q35: How would you traverse a Linked List in <i><code>O(n<sup>1/2</sup>)</code></i>? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q36: How to apply Binary Search <code><i>O</i>(<i>log n</i>)</code> on a sorted Linked List? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q37: When is doubly linked list more efficient than singly linked list? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q38: Find the length of a Linked List which contains cycle (loop) ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q39: Given a singly Linked List, determine if it is a Palindrome ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q40: How is it possible to do Binary Search on a Doubly-Linked List in <code><i>O</i>(<i>n</i>)</code> time? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q41: Why would you ever do Binary Search on a Doubly-Linked list? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q42: Do you know any better than than Floyd's algorithm for cycle detection? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q43: Copy a Linked List with Random (Arbitrary) Pointer using <code><i>O</i>(<i>1</i>)</code> Space ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Queues>Queues</a> Interview Questions
#### Q1: List some Queue real-life applications ⭐
**Answer:**
Queue, as the name suggests is used whenever we need to manage any group of objects in an order in which the first one coming in, also gets out first while the others wait for their turn, like in the following scenarios:

* Serving requests on a single shared resource, like a printer, CPU task scheduling etc.
* In real life scenario, Call Center phone systems uses Queues to hold people calling them in an order, until a service representative is free.
* Handling of interrupts in real-time systems. The interrupts are handled in the same order as they arrive i.e First come first served.

**Source:** _www.studytonight.com_

#### Q2: What is Queue? ⭐
**Answer:**
A **queue** is a container of objects (a _linear_ collection) that are inserted and removed according to the first-in first-out (FIFO) principle. The process to add an element into queue is called **Enqueue** and the process of removal of an element from queue is called **Dequeue**.

![](https://user-images.githubusercontent.com/13550565/85218641-9d2f9e80-b3ce-11ea-8c1b-a9c058057a70.png)


**Source:** _www.cs.cmu.edu_

#### Q3: Why and when should I use Stack or Queue data structures instead of Arrays/Lists? ⭐⭐
**Answer:**
Because they help manage your data in more a _particular_ way than arrays and lists. It means that when you're debugging a problem, you won't have to wonder if someone randomly inserted an element into the middle of your list, messing up some invariants.

Arrays and lists are random access. They are very flexible and also easily *corruptible*. If you want to manage your data as FIFO or LIFO it's best to use those, already implemented, collections.

More practically you should:
* Use a queue when you want to get things out in the order that you put them in (FIFO)
* Use a stack when you want to get things out in the reverse order than you put them in (LIFO)
* Use a list when you want to get anything out, regardless of when you put them in (and when you don't want them to automatically be removed).

**Source:** _stackoverflow.com_

#### Q4: What is Complexity Analysis of Queue operations?  ⭐⭐
**Answer:**
* Queues offer random access to their contents by shifting the first element off the front of the queue. You have to do this repeatedly to access an arbitrary element somewhere in the queue. Therefore, **access** is <code><i>O</i>(<i>n</i>)</code>.
* Searching for a given value in the queue requires iterating until you find it. So **search** is <code><i>O</i>(<i>n</i>)</code>.
* Inserting into a queue, by definition, can only happen at the back of the queue, similar to someone getting in line for a delicious Double-Double burger at In 'n Out. Assuming an efficient queue implementation, queue **insertion** is <code><i>O</i>(<i>1</i>)</code>.
* Deleting from a queue happens at the front of the queue. Assuming an efficient queue implementation, queue **deletion** is `<code><i>O</i>(<i>1</i>)</code>.

**Source:** _github.com_

#### Q5: What are some types of Queue? ⭐⭐
**Answer:**
 Queue can be classified into following types:

* **Simple Queue** - is a linear data structure in which removal of elements is done in the same order they were inserted i.e., the element will be removed first which is inserted first.

![](https://scanftree.com/Data_Structure/queues.png)

* **Circular Queue** - is a linear data structure in which the operations are performed based on FIFO (First In First Out) principle and the last position is connected back to the first position to make a circle. It is also called **Ring Buffer**. Circular queue avoids the wastage of space in a regular queue implementation using arrays.


![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Ring_buffer.svg/794px-Ring_buffer.svg.png)


* **Priority Queue** - is a type of queue where each element has a priority value and the deletion of the elements is depended upon the priority value

![](https://www.aoprogrammer.com/wp-content/uploads/2018/07/enqueue-priority-queue.png)

  * In case of **max-priority queue**, the element will be deleted first which has the largest priority value
  * In case of **min-priority queue** the element will be deleted first which has the minimum priority value.
* **De-queue (Double ended queue)** - allows insertion and deletion from both the ends i.e. elements can be added or removed from rear as well as front end.

![](https://i.imgur.com/AF3RVpP.png)

  * **Input restricted deque** - In input restricted double ended queue, the insertion operation is performed at only one end and deletion operation is performed at both the ends.

![](https://i.imgur.com/dSJUHFE.png)

  * **Output restricted deque** - In output restricted double ended queue, the deletion operation is performed at only one end and insertion operation is performed at both the ends.


![](https://i.imgur.com/vyHyffe.png)

 


**Source:** _www.ques10.com_

#### Q6: Implement Stack using Two Queues (with efficient `push`) ⭐⭐
**Details:**
Given two queues with their standard operations (`enqueue`, `dequeue`, `isempty`, `size`), implement a stack with its standard operations (`pop`, `push`, `isempty`, `size`). The stack should be efficient when pushing an item.

**Answer:**
Given we have `queue1` and `queue2`:

**push** - `O(1)`: 
  - enqueue in `queue1`

**pop** - `O(n)`:
  - while size of `queue1` is bigger than 1, pipe (dequeue + enqueue) dequeued items from `queue1` into `queue2`
  - dequeue and return the last item of `queue1`, then switch the names of `queue1` and `queue2`

**Source:** _stackoverflow.com_

#### Q7: Implement a Queue using two Stacks ⭐⭐
**Details:**
Suppose we have two stacks and no other temporary variable. Is to possible to "construct" a queue data structure using only the two stacks?

**Answer:**
Keep two stacks, let's call them `inbox` and `outbox`.

**Enqueue**:

 - Push the new element onto `inbox`

**Dequeue**:

 - If `outbox` is empty, refill it by popping **each** element from `inbox` and pushing it onto `outbox`
 - Pop and return the top element from `outbox`

**Source:** _stackoverflow.com_

#### Q8: What are benefits of Circular Queue? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: Name some Queue implementations and compare them by efficiency of operations ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: Compare Array-Based vs List-Based implementation of Queues ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: How to manage Full Circular Queue event? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Name most efficient way to implement Stack and Queue together? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: How implement a Queue using only One (1) Stack? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: How do I convert a Queue into the Stack? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Recursion>Recursion</a> Interview Questions
#### Q1: What is a good example of Recursion (other than generating a Fibonacci sequence)? ⭐⭐
**Answer:**
There are some:
* The binary tree search
* Check for a palyndrome
* Finding factorial
* Traversing the folder hierarchy of a directory tree as part of a file system
* Towers of Hanoi
* Merge sort 
* Catalan numbers

**Source:** _stackoverflow.com_

#### Q2: How Dynamic Programming is different from Recursion and Memoization? ⭐⭐
**Answer:**
* **Memoization** is when you store previous results of a function call (a real function always returns the same thing, given the same inputs). It doesn't make a difference for algorithmic complexity before the results are stored.
* **Recursion** is the method of a function calling itself, usually with a smaller dataset. Since most recursive functions can be converted to similar iterative functions, this doesn't make a difference for algorithmic complexity either.
* **Dynamic programming** is the process of solving easier-to-solve sub-problems and building up the answer from that. Most DP algorithms will be in the running times between a Greedy algorithm (if one exists) and an exponential (enumerate all possibilities and find the best one) algorithm.
  * DP algorithms could be implemented with recursion, but they don't have to be.
  * DP algorithms can't be sped up by memoization, since each sub-problem is only ever solved (or the "solve" function called) once.

**Source:** _stackoverflow.com_

#### Q3: What is the difference between Backtracking and Recursion? ⭐⭐
**Answer:**
* **Recursion** describes the calling of the _same function_ that you are in. The typical example of a recursive function is the factorial. You always need a condition that makes recursion stop (base case). 
* **Backtracking** is when the algorithm makes an opportunistic decision<sup>*</sup>, which may come up to be wrong. If the decision was wrong then the backtracking algorithm restores the state before the decision. It builds candidates for the solution and abandons those which cannot fulfill the conditions. A typical example for a task to solve would be the _Eight Queens Puzzle_. Backtracking is also commonly used within _Neuronal Networks_. Many times backtracking is not implemented recursively. If backtracking uses recursion its called **Recursive Backtracking**

P.S. <sup>*</sup> **Opportunistic decision** making refers to a process where a person or group assesses alternative actions made possible by the favorable convergence of immediate circumstances recognized **without** reference to any **general plan**.

**Source:** _www.quora.com_

#### Q4: Can you convert this Recursion function into a loop? ⭐⭐
**Details:**
Can you convert this recursion function into a loop?
```js
A(x) {
  if x<0 return 0;
  return something(x) + A(x-1)
}
```

**Answer:**
Any recursive function can be made to iterate (into a loop) but you need to use a stack yourself to keep the state.

```js
A(x) {
  temp = 0;
  for i in 0..x {
    temp = temp + something(i);
  }
  return temp;
}
```

**Source:** _stackoverflow.com_

#### Q5: Explain what is DFS (Depth First Search) algorithm for a Graph and how does it work? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: Convert a Binary Tree to a Doubly Linked List ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: How to use Memoization for N-th Fibonacci number?  ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: How to recursively reverse a Linked List? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: Is it always possible to write a non-recursive form for every Recursive function? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Searching>Searching</a> Interview Questions
#### Q1: Explain what is Binary Search ⭐⭐
**Answer:**
When the list is **sorted** we can use the **binary search** (also known as half-interval search, logarithmic search, or binary chop) technique to find items on the list. Here's a step\-by\-step description of using binary search:

1.  Let `min = 1` and `max = n`.
2.  Guess the average of `max` and `min`  **rounded down** so that it is an integer.
3.  If you guessed the number, stop. You found it!
4.  If the guess was too low, set _min_ to be one larger than the guess.
5.  If the guess was too high, set _max_ to be one smaller than the guess.
6.  Go back to step two.

In this example we looking for array item with value `4`:
![](https://upload.wikimedia.org/wikipedia/commons/thumb/6/64/Binary_search_into_array_-_example.svg/382px-Binary_search_into_array_-_example.svg.png)

When you do one operation in binary search we reduce the size of the problem **by half** (look at the picture below how do we reduce the size of the problem area) hence the complexity of binary search is <code><i>O</i>(<i>log n</i>)</code>. The binary search algorithm can be written either _recursively_ or _iteratively_.

![](https://dirask.com/static/bucket/1575232592915-67oY6qqQE1--binarry_search_algorithm.png)

**Source:** _www.tutorialspoint.com_

#### Q2: Explain what is Linear (Sequential) Search and when may we use one? ⭐⭐
**Answer:**
**Linear (sequential) search** goes through all possible elements in some array and compare each one with the desired element. It may take up to <code><i>O</i>(<i>n</i>)</code> operations, where N is the size of an array and is widely considered to be horribly slow. In linear search when you perform one operation you reduce the size of the problem _by one_ (when you do one operation in binary search you reduce the size of the problem _by half_). Despite it, it can still be used when:

* You need to perform this search only once,
* You are _forbidden_ to rearrange the elements and you do not have any extra memory,
* The array is tiny, such as ten elements or less, or the performance is not an issue at all,
* Even though in theory other search algorithms may be faster than linear search (for instance binary search), in practice even on medium-sized arrays (around 100 items or less) it might be infeasible to use anything else. On larger arrays, it only makes sense to use other, faster search methods if the data is large enough, because the initial time to prepare (sort) the data is comparable to many linear searches,
* When the list items are arranged in order of _decreasing probability_, and these probabilities are geometrically distributed, the cost of linear search is only <code><i>O</i>(<i>1</i>)</code>
* You have no idea what you are searching.

When you ask MySQL something like `SELECT x FROM y WHERE z = t`, and `z` is a column _without_ an index, linear search is performed with all the consequences of it. This is why adding an index to _searchable_ columns is important.

**Source:** _bytescout.com_

#### Q3: Explain some Linear Search optimization techniques ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q4: Recursive and Iterative Binary Search: Which one is more efficient and why? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q5: Explain what is Interpolation Search ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: Write a program for Recursive Binary Search ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: What's wrong with this Recursive Binary Search function? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: Compare Binary Search vs Linear Search ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: What is an example of Interpolation Search being slower than Binary Search? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: Which of the following algorithms would be the fastest? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: What is a Jump (or Block) Search? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Explain why complexity of Binary Search is <code><i>O</i>(<i>log n</i>)</code>? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: Explain how does the Sentinel Search work? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: For Binary Search why do we need round down the average? Could we round up instead? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: Explain what is Fibonacci Search technique? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: How to apply Binary Search <code><i>O</i>(<i>log n</i>)</code> on a sorted Linked List? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: Explain when and how to use Exponential (aka Doubling or Galloping) Search?  ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: What is the optimal block size for a Jump Search? Explain. ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: Explain what is Ternary Search? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q20: How is it possible to do Binary Search on a Doubly-Linked List in <code><i>O</i>(<i>n</i>)</code> time? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q21: Why would you ever do Binary Search on a Doubly-Linked list? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q22: Is Sentinel Linear Search better than normal Linear Search? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q23: Why use Binary Search if there's ternary search? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q24: When Jump Search is a better alternative than a Binary Search? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Sorting>Sorting</a> Interview Questions
#### Q1: Explain how Bubble Sort works ⭐
**Answer:**
**Bubble Sort** is based on the idea of repeatedly _comparing_ pairs of adjacent elements and then swapping their positions if they are in the wrong order. Bubble sort is a _stable_, _in-place_ sort algorithm.

How it works:
* In an unsorted array of `n` elements, start with the first two elements and sort them in ascending order. (Compare the element to check which one is greater).
* Compare the second and third element to check which one is greater, and sort them in ascending order.
* Compare the third and fourth element to check which one is greater, and sort them in ascending order.
* ...
* Repeat steps 1–`n` until no more swaps are required.

**Visualisation:**


![](https://camo.githubusercontent.com/383b23979d4d7f279f8fb285b36bcdd357b10a35/68747470733a2f2f75706c6f61642e77696b696d656469612e6f72672f77696b6970656469612f636f6d6d6f6e732f632f63382f427562626c652d736f72742d6578616d706c652d33303070782e676966)


**Source:** _github.com_

#### Q2: Why Sorting algorithms are important? ⭐
**Answer:**
Efficient sorting is important for **optimizing the efficiency of other algorithms** (such as search and merge algorithms) that require input data to be in sorted lists. Sorting is also often useful for canonicalizing data and for producing human-readable output. Sorting have direct applications in database algorithms, divide and conquer methods, data structure algorithms, and many more.

**Source:** _en.wikipedia.org_

#### Q3: What is meant by to "Sort in Place"? ⭐⭐
**Answer:**
The idea of an in-place algorithm isn't unique to sorting, but sorting is probably the most important case, or at least the most well-known. The idea is about space efficiency - using the minimum amount of RAM, hard disk or other storage that you can get away with. 

The idea is to **produce an output in the same memory space that contains the input** by successively transforming that data until the output is produced. This avoids the need to use twice the storage - one area for the input and an equal-sized area for the output.

**Quicksort** is one example of In-Place Sorting.

**Source:** _stackoverflow.com_

#### Q4: Explain what is ideal Sorting algorithm? ⭐⭐
**Answer:**
The **ideal sorting algorithm** would have the following properties:

* **Stable**: Equal keys aren’t reordered.
* **Operates in place:** requiring O(1) extra space.
* Worst-case `O(n log n)` key comparisons.
* Worst-case `O(n)` swaps.
* **Adaptive**: Speeds up to O(n) when data is nearly sorted or when there are few unique keys.

There is **no** algorithm that has all of these properties, and so the choice of sorting algorithm depends on the application.

**Source:** _www.toptal.com_

#### Q5: Classify Sorting Algorithms ⭐⭐
**Answer:**
Sorting algorithms can be categorised based on the following parameters:

1.  **Based on Number of Swaps or Inversion**. This is the number of times the algorithm swaps elements to sort the input. `Selection Sort` requires the minimum number of swaps.
2.  **Based on Number of Comparisons**. This is the number of times the algorithm compares elements to sort the input. Using Big-O notation, the sorting algorithm examples listed above require at least <code><i>O</i>(<i>n log n</i>)</code> comparisons in the best case and <code><i>O</i>(<i>n</i><sup>2</sup>)</code> comparisons in the worst case for most of the outputs.
3.  **Based on Recursion or Non-Recursion**. Some sorting algorithms, such as `Quick Sort`, use recursive techniques to sort the input. Other sorting algorithms, such as `Selection Sort` or `Insertion Sort`, use non-recursive techniques. Finally, some sorting algorithm, such as `Merge Sort`, make use of both recursive as well as non-recursive techniques to sort the input.
4.  **Based on Stability**. Sorting algorithms are said to be `stable` if the algorithm maintains the relative order of elements with equal keys. In other words, two equivalent elements remain in the same order in the sorted output as they were in the input.
    *  `Insertion sort`, `Merge Sort`, and `Bubble Sort` are stable
    *  `Heap Sort` and `Quick Sort` are not stable
5.  **Based on Extra Space Requirement.** Sorting algorithms are said to be _in place_ if they require a constant <code><i>O</i>(<i>1</i>)</code> extra space for sorting.
    *  `Insertion sort` and `Quick-sort` are `in place` sort as we move the elements about the pivot and do not actually use a separate array which is NOT the case in merge sort where the size of the input must be allocated beforehand to store the output during the sort.
    *  `Merge Sort` is an example of `out place` sort as it require extra memory space for it’s operations.

**Source:** _www.freecodecamp.org_

#### Q6: Explain how Insertion Sort works ⭐⭐
**Answer:**
**Insertion Sort** is an _in-place_, _stable_, _comparison-based_ sorting algorithm. The idea is to maintain a sub-list which is always sorted. An element which is to be 'insert'ed in this sorted sub-list, has to find its appropriate place and then it has to be inserted there. Hence the name, **insertion sort**.

Steps on how it works:
* If it is the first element, it is already sorted.
* Pick the next element.
* Compare with all the elements in sorted sub-list.
* Shift all the the elements in sorted sub-list that is greater than the value to be sorted.
* Insert the value.
* Repeat until list is sorted.

**Visualisation:**


![](https://upload.wikimedia.org/wikipedia/commons/0/0f/Insertion-sort-example-300px.gif)

**Source:** _medium.com_

#### Q7: What are advantages and disadvantages of Bubble Sort? ⭐⭐
**Answer:**
**Advantages:**

* Simple to understand
* Ability to detect that the list is sorted efficiently is built into the algorithm. When the list is already sorted (best-case), the complexity of bubble sort is only `O(n)`. 


**Disadvantages:**
* It is very slow and runs in `O(n^2)` time in worst as well as average case. Because of that Bubble sort does not deal well with a large set of data. For example Bubble sort is three times slower than **Quicksort** even for n = 100



**Source:** _en.wikipedia.org_

#### Q8: How would you optimise Bubble Sort? ⭐⭐
**Answer:**
In Bubble sort, you know that after `k` passes, the largest `k` elements are sorted at the `k` last entries of the array, so the conventional Bubble sort uses:
```java
public static void bubblesort(int[] a) {
  for (int i = 1; i < a.length; i++) {
    boolean is_sorted = true;

    for (int j = 0; j < a.length - i; j++) { // skip the already sorted largest elements, compare to a.length - 1
      if (a[j] > a[j+1]) {
         int temp = a[j];
         a[j] = a[j+1];
         a[j+1] = temp;
         is_sorted = false;
      }
    }

    if(is_sorted) return;
  }
}
```
Now, that would still do a lot of unnecessary iterations when the array has a long sorted tail of largest elements. If you remember where you made your _last swap_, you know that after that index, there are the largest elements in order, so:

```java
public static void bubblesort(int[] a) {
  int lastSwap = a.length - 1;
  for (int i = 1; i< a.length; i++) {
    boolean is_sorted = true;
    int currentSwap = -1;

    for (int j = 0; j < lastSwap; j++) { // compare to a.length - i
      if (a[j] > a[j+1]) {
         int temp = a[j];
         a[j] = a[j+1];
         a[j+1] = temp;
         is_sorted = false;
         currentSwap = j;
      }
    }

    if (is_sorted) return;
    lastSwap = currentSwap;
  }
}
```
This allows to skip over many elements, resulting in about a worst case 50% improvement in comparison count (though no improvement in swap counts), and adds very little complexity.

**Source:** _stackoverflow.com_

#### Q9: Insert an item in a sorted Linked List maintaining order ⭐⭐
**Answer:**
The `add()` method below walks down the list until it finds the appropriate position. Then, it splices in the new node and updates the `start`, `prev`, and `curr` pointers where applicable.

Note that the reverse operation, namely _removing_ elements, doesn't need to change, because you are simply throwing things away which would not change any order in the list.


**Source:** _stackoverflow.com_

#### Q10: What's the difference between External vs Internal sorting? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: Explain how Merge Sort works ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Which sort algorithm works best on mostly sorted data? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: Why would you use Merge Sort for a Linked List? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: Explain how Heap Sort works ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: When is each Sorting algorithm used? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: When is Quicksort better than Mergesort? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: What is "stability" in sorting algorithms and why is it important? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: Sort a Stack using Recursion ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: Sort a Stack using another Stack ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q20: Which of the following algorithms would be the fastest? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q21: Why is Merge sort preferred over Quick sort for sorting Linked Lists? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q22: Explain how Radix Sort works ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q23: Explain how QuickSort works ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q24: Explain how to find 100 largest numbers out of an array of 1 billion numbers ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q25: When Merge Sort is preferred over Quick Sort? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q26: How can I pair socks from a pile efficiently? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Stacks>Stacks</a> Interview Questions
#### Q1: Define Stack ⭐
**Answer:**
A **Stack** is a container of objects that are inserted and removed according to the last-in first-out (**LIFO**) principle. In the pushdown stacks only two operations are allowed: push the item into the stack, and pop the item out of the stack.

There are basically three operations that can be performed on stacks. They are:
 
1. inserting an item into a stack (**push**). 
2. deleting an item from the stack (**pop**). 
3. displaying the contents of the stack (**peek** or **top**).

A stack is a limited access data structure - elements can be added and removed from the stack only at the top. push adds an item to the top of the stack, pop removes the item from the top. A helpful analogy is to think of a stack of books; you can remove only the top book, also you can add a new book on the top.

![](https://user-images.githubusercontent.com/13550565/85218531-fea33d80-b3cd-11ea-8ba4-77c37d446d07.png)


**Source:** _www.cs.cmu.edu_

#### Q2: Explain why Stack is a recursive data structure ⭐
**Answer:**
A **stack** is a **recursive** data structure, so it's:

* a stack is either empty or
* it consists of a top and the rest which is a stack by itself;

**Source:** _www.cs.cmu.edu_

#### Q3: Why and when should I use Stack or Queue data structures instead of Arrays/Lists? ⭐⭐
**Answer:**
Because they help manage your data in more a _particular_ way than arrays and lists. It means that when you're debugging a problem, you won't have to wonder if someone randomly inserted an element into the middle of your list, messing up some invariants.

Arrays and lists are random access. They are very flexible and also easily *corruptible*. If you want to manage your data as FIFO or LIFO it's best to use those, already implemented, collections.

More practically you should:
* Use a queue when you want to get things out in the order that you put them in (FIFO)
* Use a stack when you want to get things out in the reverse order than you put them in (LIFO)
* Use a list when you want to get anything out, regardless of when you put them in (and when you don't want them to automatically be removed).

**Source:** _stackoverflow.com_

#### Q4: Implement Stack using Two Queues (with efficient `push`) ⭐⭐
**Details:**
Given two queues with their standard operations (`enqueue`, `dequeue`, `isempty`, `size`), implement a stack with its standard operations (`pop`, `push`, `isempty`, `size`). The stack should be efficient when pushing an item.

**Answer:**
Given we have `queue1` and `queue2`:

**push** - `O(1)`: 
  - enqueue in `queue1`

**pop** - `O(n)`:
  - while size of `queue1` is bigger than 1, pipe (dequeue + enqueue) dequeued items from `queue1` into `queue2`
  - dequeue and return the last item of `queue1`, then switch the names of `queue1` and `queue2`

**Source:** _stackoverflow.com_

#### Q5: Implement a Queue using two Stacks ⭐⭐
**Details:**
Suppose we have two stacks and no other temporary variable. Is to possible to "construct" a queue data structure using only the two stacks?

**Answer:**
Keep two stacks, let's call them `inbox` and `outbox`.

**Enqueue**:

 - Push the new element onto `inbox`

**Dequeue**:

 - If `outbox` is empty, refill it by popping **each** element from `inbox` and pushing it onto `outbox`
 - Pop and return the top element from `outbox`

**Source:** _stackoverflow.com_

#### Q6: What is complexity of `push` and `pop` for a Stack implemented using a LinkedList? ⭐⭐
**Answer:**
<code><i>O</i>(<i>1</i>)</code>. Note, you don't have to insert at the end of the list. If you insert at the front of a (singly-linked) list, they are both `O(1)`.

Stack contains 1,2,3:

```py
[1]->[2]->[3]
```

Push 5:

```js
[5]->[1]->[2]->[3]
```

Pop:

```js
[1]->[2]->[3] // returning 5
```


**Source:** _stackoverflow.com_

#### Q7: Design a Stack that supports retrieving the min element in _`O(1)`_ ⭐⭐
**Details:**
Design a stack that supports push, pop, top, and retrieving the minimum element in constant time.

* `push(x)` - Push element x onto stack.
* `pop()` - Removes the element on top of the stack.
* `top()` - Get the top element.
* `getMin()` - Retrieve the **minimum** element in the stack.

**Answer:**
Using a linked list store the current minimum value. When you add a new number it looks at the previous min and changes the current min to the current value if the current value is lower. Note, each node stores the `min` value _at or below_ it so we don't need to recalculate `min` on pop.

#### Q8: Reverse a String using Stack ⭐⭐
**Answer:**
The followings are the steps to reversing a String using Stack:

1.  `String` to `char[]`.
2.  Create a `Stack`.
3.  **Push** all characters, one by one.
4.  Then **Pop** all characters, one by one and put into the `char[]`.
5.  Finally, convert to the `String`.

#### Q9: Why Are Stacks Useful? ⭐⭐
**Answer:**
They’re very useful because they afford you constant time <code><i>O</i>(<i>1</i>)</code> operations when _inserting_ or _removing_ from the front of a data structure. One common use of a stack is in compilers, where a stack can be used to make sure that the brackets and parentheses in a code file are all balanced, i.e., have an opening and closing counterpart. Stacks are also very useful in evaluating mathematical expressions. 

**Source:** _medium.com_

#### Q10: How to implement Linked List Using Stack? ⭐⭐
**Answer:**
You can simulate a linked list by using two stacks. One stack is the "list," and the other is used for temporary storage.

* To **add** an item at the head, simply push the item onto the stack. 
* To **remove** from the head, pop from the stack.
* To **insert** into the middle somewhere, pop items from the "list" stack and push them onto the temporary stack until you get to your insertion point. Push the new item onto the "list" stack, then pop from the temporary stack and push back onto the "list" stack. Deletion of an arbitrary node is similar.

This isn't terribly efficient, by the way, but it would in fact work.

**Source:** _stackoverflow.com_

#### Q11: Compare Array based vs Linked List stack implementations ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: Implement Double Linked List from Stack with min complexity ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: How reverse Stack without using any (extra) data structure? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: Find duplicate parenthesis in expression ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: Explain what are Infix, Prefix and Postfix Expressions? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: Sort a Stack using Recursion ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: Sort a Stack using another Stack ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: Check if parentheses are balanced using Stack ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: Why do we need Prefix and Postfix notations? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q20: Given an extremely large file that contains parenthesis, how would you say that the parenthesis are balanced? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q21: How to implement 3 Stacks with one Array? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q22: Build a Binary Expression Tree for this expression ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q23: How implement a Queue using only One (1) Stack? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q24: How do I convert a Queue into the Stack? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q25: How to check for braces balance in a really large (1T) file in parallel? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Strings>Strings</a> Interview Questions
#### Q1: What is String in Data Structures? ⭐
**Answer:**
A **string** is generally considered as a **data type** and is often implemented as an **array data structure** of bytes (or words) that stores a sequence of elements, typically characters, using some character encoding. String may also denote more general arrays or other sequence (or list) data types and structures.

**Source:** _dev.to_

#### Q2: What is the difference between Strings vs. Char arrays? ⭐⭐
**Answer:**
**Char arrays**: 
* Static-sized
* Fast access
* Few built-in methods to manipulate strings
* A char array doesn’t define a data type

**Strings**:
* Slower access
* Define a data type
* Dynamic allocation
* More built-in functions to support string manipulations

**Source:** _dev.to_

#### Q3: Reverse a String using Stack ⭐⭐
**Answer:**
The followings are the steps to reversing a String using Stack:

1.  `String` to `char[]`.
2.  Create a `Stack`.
3.  **Push** all characters, one by one.
4.  Then **Pop** all characters, one by one and put into the `char[]`.
5.  Finally, convert to the `String`.

#### Q4: What is strings mutability and immutability? ⭐⭐
**Answer:**
Strings can either be **mutable** or **immutable**. 
* When a string is **immutable** it means that it's fixed allocated. So your string it's unique and can't be modified. If you change it, a copy of that string is created and the original string is deallocated instead. 
* When a string is **mutable** it means that it's dynamically allocated, so your string can be modified.

**Source:** _dev.to_

#### Q5: What is a null-terminated String? ⭐⭐
**Answer:**
A "string" is really just an array of `char`s; a null-terminated string is one where a null character `'\0'` marks the end of the string (not necessarily the end of the array). All strings in code (delimited by double quotes `""`) are automatically null-terminated by the compiler.

So for example, `"hi"` is the same as `{'h', 'i', '\0'}`.

Null-terminated strings are often a _drain on performance_, for the obvious reason that the time taken to discover the length depends on the length. The usual solution is to do both - keep the length and maintain the null terminator. It's not much extra work and means that you are always ready to pass the string to any function.

**Source:** _stackoverflow.com_

#### Q6: Mentions some pros and cons of immutable vs mutable Strings ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: Remove Invalid Parentheses ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: How to check if two Strings (words) are Anagrams? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: How to check if String is a Palindrome? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: Find all the Permutations of a String ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: Reverse the ordering of words in a String ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: What are Pascal Strings? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: What is Rope Data Structure is used for? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: Explain Knuth-Morris-Pratt (KMP) Algorithm in Plain English ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: Why is `char[]` preferred over String for passwords? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: Check for balanced parentheses in linear time using constant space ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: What are some advantages of Rope data structure? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18: What are some limitations of Ropes? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: Explain Boyer-Moore Algorithm with Example ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q20: When to use Ropes over StringBuilders? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q21: When is Rabin-Karp more effective than KMP or Boyer-Moore? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q22: What are the main differences between the Knuth-Morris-Pratt search algorithm and the Boyer-Moore search algorithm? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q23: What's the rationale for `null` terminated strings? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q24: Compare Strings vs Ropes from the Performance Analysis ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q25: Find all the repeating substrings in a given String (or DNA chromosome sequence) ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Trees>Trees</a> Interview Questions
#### Q1: Define Tree Data Structure ⭐
**Answer:**
**Trees** are well-known as a _non-linear_ data structure. They don’t store data in a linear way. They organize data _hierarchically_.

A **tree** is a collection of entities called **nodes**. Nodes are connected by **edges**. Each node contains a **value** or **data** or **key**, and it may or may not have a **child** node. The first node of the tree is called the **root**. **Leaves** are the last nodes on a tree. They are nodes without children.



![](https://miro.medium.com/max/975/1*PWJiwTxRdQy8A_Y0hAv5Eg.png)


**Source:** _www.freecodecamp.org_

#### Q2: Define Binary Tree ⭐
**Answer:**
A normal tree has no restrictions on the number of children each node can have. A **binary tree** is made of nodes, where each node contains a "left" pointer, a "right" pointer, and a data element. 

There are three different types of binary trees:

* **Full binary tree**: Every node other than leaf nodes has 2 child nodes.
* **Complete binary tree**: All levels are filled except possibly the last one, and all nodes are filled in as far left as possible.
* **Perfect binary tree**: All nodes have two children and all leaves are at the same level.



![](https://study.com/cimages/multimages/16/0e0646ba-30e5-40d9-b45c-a138f038f05b_full_complete_perfect.png)



**Source:** _study.com_

#### Q3: What is Height and Depth of a Tree and its Nodes? ⭐⭐
**Answer:**
* The **depth of a node** is the length of the _path to its root_
* The **height of a node** is the number of edges on the longest path from the node to a leaf
* The **height of a tree** is the length of the _longest path to a leaf_

<br/>

![](https://www.growingwiththeweb.com/images/data-structures/avl-tree/height-vs-depth.svg)



**Source:** _medium.com_

#### Q4: What is Binary Search Tree? ⭐⭐
**Answer:**
**Binary search tree** is a data structure that quickly allows to maintain a _sorted list_ of numbers.

* It is called a _binary tree_ because each tree node has maximum of two children.
* It is called a _search tree_ because it can be used to search for the presence of a number in `O(log n)` time.

The properties that separates a binary search tree from a regular binary tree are:

* All nodes of left subtree are less than root node
* All nodes of right subtree are more than root node
* Both subtrees of each node are also BSTs i.e. they have the above two properties


![](https://cdn.programiz.com/sites/tutorial2program/files/bst-vs-not-bst.jpg)


**Source:** _www.programiz.com_

#### Q5: How to implement a tree data-structure? Provide some code. ⭐⭐
**Answer:**
That is a basic (generic) tree structure that can be used for `String` or any other object:

**Source:** _stackoverflow.com_

#### Q6: What's the difference between the data structure Tree and Graph? ⭐⭐
**Answer:**
**Graph:**
* Consists of a set of vertices (or nodes) and a set of edges connecting some or all of them
* Any edge can connect any two vertices that aren't already connected by an identical edge (in the same direction, in the case of a directed graph)
* Doesn't have to be connected (the edges don't have to connect all vertices together): a single graph can consist of a few disconnected sets of vertices
* Could be directed or undirected (which would apply to all edges in the graph)

**Tree:**
* A type of graph (fit with in the category of Directed Acyclic Graphs (or a DAG))
* Vertices are more commonly called "nodes"
* Edges are directed and represent an "is child of" (or "is parent of") relationship
* Each node (except the root node) has exactly one parent (and zero or more children)
* Has exactly one "root" node (if the tree has at least one node), which is a node without a parent
* Has to be connected
* Is acyclic, meaning it has no cycles: "a cycle is a path [AKA sequence] of edges and vertices wherein a vertex is reachable from itself"
* Trees aren't a recursive data structure



![](https://miro.medium.com/max/2262/1*-yHATwTlY2hwceJ93-D-cw.jpeg)


**Source:** _stackoverflow.com_

#### Q7: What is the difference between Tree Depth and Height? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: Explain the difference between Binary Tree and Binary Search Tree with an example? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q9: Provide some practical examples of using Depth-First Search (DFS) vs Breadth-First Search (BFS)? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q10: Why do we want to use Binary Search Tree? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q11: What is AVL Tree? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q12: What are advantages and disadvantages of BST? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q13: What is Balanced Tree and why is that important? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q14: What is Diameter of a Tree? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q15: What is the difference between Heap and Red-Black Tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q16: Explain how to balance AVL Tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q17: How does inserting or deleting nodes affect a Red-Black tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q18:  Explain what the main differences between red-black (RB) trees and AVL trees ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q19: What is Red-Black tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q20: What is the time complexity for insert into Red-Black Tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q21: Explain what is B-Tree? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q22: How do we know whether we need to use BSF or DSF algorithm? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q23: Is there any reason anyone should use BSTs instead of AVLs in the first place? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q24: Why does a Breadth First Search (BFS) use more memory than Depth First Search (DFS)? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q25: Explain a B-Tree data structure for 5 years old ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q26: What's the main reason for choosing Red Black (RB) trees instead of AVL trees? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q27: Why is a Hash Table not used instead of a B-Tree in order to access data inside a database? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q28: How is an AVL tree different from a B-tree? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q29: What are the differences between B trees and B+ trees? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q30: How are B-Trees used in practice? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q31: Why do we need a separate datastructure like B-Tree for database and file system? ⭐⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

## [[⬆]](#toc) <a name=Trie>Trie</a> Interview Questions
#### Q1: What is Trie? ⭐
**Answer:**
**Trie** (also called **digital tree **or **prefix tree**) is a _tree-based data structure_, which is used for efficient _retrieval_ of a key in a large data-set of strings. Unlike a binary search tree, no node in the tree stores the key associated with that node; instead, its position in the tree defines the key with which it is associated; i.e., **the value of the key is distributed across the structure**. All the descendants of a node have a common prefix of the string associated with that node, and the root is associated with the empty string. Each complete English word has an arbitrary integer value associated with it (see image).

<br/>

![](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ae/Patricia_trie.svg/1200px-Patricia_trie.svg.png)
<br/>

**Source:** _medium.com_

#### Q2: What are some Trie implementation strategies? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q3: Name some application of Trie data structure ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q4: What are some advantages and disadvantages of Trie? ⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q5: Compare lookup operation in Trie vs Hash Table ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q6: What are some main advantages of Tries over Hash Tables ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q7: How To Choose Between a Hash Table and a Trie (Prefix Tree)? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>

#### Q8: What are main advantages of Tries over Binary Search Trees (BSTs)? ⭐⭐⭐⭐
Read answer on 👉 <a href='https://www.fullstack.cafe'>FullStack.Cafe</a>



