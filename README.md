# Leetcode
## Linked List Concept

A **linked list** is a linear data structure where each element, known as a node, contains both the actual data and a reference (or "link") to the next node in the sequence. The main types are singly linked list, doubly linked list, and circular linked list. In a singly linked list, each node points to the next node; in a doubly linked list, each node points to both the next and previous node[1][2][3][4].

### Key Features
- **Dynamic size:** Grows or shrinks during runtime.
- **Efficient insertion/deletion:** Particularly at the beginning or middle.
- **Sequential access:** No direct access by index, unlike arrays—must traverse nodes in order.

## Linked List: Time and Space Complexity

Here's a summary table for common singly linked list operations:

| Operation                | Time Complexity | Space Complexity | Notes                                       |
|--------------------------|----------------|------------------|---------------------------------------------|
| Insertion at head        | O(1)           | O(1)             | Constant time, pointer change only[5]       |
| Insertion at end         | O(n)           | O(1)             | Traverse to end, then insert[5]             |
| Insertion at position    | O(n)           | O(1)             | Traverse to position, then insert[5]        |
| Deletion at head         | O(1)           | O(1)             | Constant time, pointer updated[5]           |
| Deletion at end          | O(n)           | O(1)             | Need to traverse to second-last node[5]     |
| Deletion at position     | O(n)           | O(1)             | Traverse to position, then delete[5]        |
| Searching (by value)     | O(n)           | O(1)             | Sequential traversal[5][6]                 |
| Traversal (iterate all)  | O(n)           | O(1)             | Must visit all nodes once                   |
| Space (total for list)   | O(n)           |                  | n = number of nodes, each has value+pointer[7] |

### Explanation:
- **Insertion at Head:** You only need to update a few pointers; doesn't depend on the number of nodes[5].
- **Insertion/Deletion at End or Position:** Requires traversal (linear with list size)[5].
- **Search:** No indexing — you must traverse in sequence, so O(n)[7][5].
- **Space:** Each node stores data and at least one pointer—total memory grows linearly with node count[7].

## Example: Reversing a Linked List

- **Time Complexity:** O(n), since each node is visited once.
- **Space Complexity:** O(1), as only a few extra pointers are used regardless of list size (excluding recursive methods)[8][9].

## Linked List Practice Problems (with Time & Space Complexity)

Below are some classic problems and their analyses:

| Problem                                 | Time Complexity | Space Complexity | Notes                                         |
|------------------------------------------|----------------|------------------|-----------------------------------------------|
| Find middle of linked list               | O(n)           | O(1)             | Two pointer technique                         |
| Reverse linked list (iterative)          | O(n)           | O(1)             | No new nodes created, just pointer changes    |
| Detect cycle in linked list              | O(n)           | O(1)             | Floyd’s Cycle Detection (Tortoise & Hare)[10]  |
| Merge two sorted linked lists            | O(n+m)         | O(1)             | n, m are lengths of the lists[11]             |
| Remove N-th node from end                | O(n)           | O(1)             | Single traversal with two pointers            |
| Palindrome check (using stack)           | O(n)           | O(n)             | Uses additional stack for values              |
| Palindrome check (reverse half, in-place)| O(n)           | O(1)             | No extra space; modifies list temporarily     |
| Length of linked list                    | O(n)           | O(1)             | Traverse and count                            |

## How Linked List Problems are Evaluated

- **Time Complexity** focuses on how many nodes/steps must be processed or traversed.
- **Space Complexity** is the additional memory (excluding the actual list) your algorithm needs.
- For most in-place manipulations (like reversal), the auxiliary space is O(1), but if you use data structures like stacks for help, it may become O(n)[8][9].

## Conclusion

Linked lists are a versatile and important concept in data structures with operations whose time and space complexities are crucial in evaluating their performance—especially for insertions, deletions, searching, and traversal. Most operations have **O(n)** time complexity except insertion/deletion at the head, which is **O(1)**, and almost all implementations use **O(1)** extra (auxiliary) space, except when extra structures (like stacks) are used[7][5][8][9].

[1] https://www.geeksforgeeks.org/dsa/linked-list-data-structure/
[2] https://www.w3schools.com/dsa/dsa_theory_linkedlists.php
[3] https://en.wikipedia.org/wiki/Linked_list
[4] https://www.programiz.com/dsa/linked-list
[5] https://www.geeksforgeeks.org/dsa/time-and-space-complexity-of-linked-list/
[6] https://stackoverflow.com/questions/35491488/linkedlist-searching-time-complexity-in-java
[7] https://brilliant.org/wiki/linked-lists/
[8] https://www.reddit.com/r/learnprogramming/comments/n1muvs/why_is_space_complexity_of_reversing_a_linked/
[9] https://www.freecodecamp.org/news/what-is-a-linked-list-types-and-examples/
[10] https://www.enjoyalgorithms.com/blog/detect-loop-in-linked-list/
[11] https://www.geeksforgeeks.org/dsa/top-50-linked-list-interview-question/
[12] https://www.tutorialspoint.com/data_structures_algorithms/linked_list_algorithms.htm
[13] https://www.freecodecamp.org/news/how-linked-lists-work/
[14] https://www.codechef.com/learn/course/linked-lists/LINKEDLIST01/problems/LINK01P01
[15] https://programiz.pro/resources/dsa-linked-list-complexity/
[16] https://stackoverflow.com/questions/72254538/space-complexity-for-linked-list
[17] https://www.simplilearn.com/tutorials/data-structure-tutorial/types-of-linked-list
[18] https://stackoverflow.com/questions/69969390/what-is-the-space-complexity-of-my-code-linked-list
[19] https://www.youtube.com/watch?v=N6dOwBde7-M
[20] https://dev.to/masakifukunishi/understanding-linked-lists-features-pros-cons-and-time-complexity-235a
