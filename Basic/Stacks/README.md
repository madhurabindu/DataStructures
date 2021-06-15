# Stacks Data Structure

## Overview
Stack is an ordered list of similar data type.
The stack is a linear data structure which follows the last in first out (LIFO) principle.
- Size of stack changes with each  and  operation. Each  and  operation increases and decreases the size of the stack by , respectively.
- Stack is said to be in Overflow state when it is completely full and is said to be in Underflow state if it is completely empty
- Abstract Data type which can be implemented using Arrays or Linked List

## Operations

![Time Complexity](./operations.png)

Implementation can be Array based on Linked List based

Array Based Operation
- Push Operation : O(1)
- Pop Operation : O(1)
- Top Operation : O(1)
- Search Operation : O(n)

Linked list based Operation
- Push Operation : O(1)
- Pop Operation : O(1)
- Top Operation : O(1)
- Search Operation : O(n)

![Time Complexity](./abc.png)


## When to Use
- The stack is mostly used in converting and evaluating expressions with infix, prefix, postfix
- Undo and Redo in games & text editors
- Browser back button
- Recursion
- Expression Evaluation and Conversion https://www.simplilearn.com/tutorials/data-structure-tutorial/stacks-in-data-structures
- Backtracking
- Function Call
- Parentheses Checking
- String Reversal
- Syntax Parsing
- Memory Management
- Many others here https://en.wikibooks.org/wiki/Data_Structures/Stacks_and_Queues
## Pros and Cons

#### Array based implementation

Pros: This is easy to implement, and memory is saved since pointers are not involved.
Cons: This is not dynamic, meaning that it can't grow and shrink depending on needs at runtime.


#### Linked list based implementation:

Pros: The linked list implementation of stack can grow and shrink according to the needs at runtime.
Cons: This requires extra memory since it uses pointers.

### Alternate
NA

## Resources
https://www.geeksforgeeks.org/stack-data-structure-introduction-program/

