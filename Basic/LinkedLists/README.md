# Linked Lists Data Structure

## Overview
Linked lists are linear data structures that hold data in individual objects called nodes. These nodes hold both the data and a reference to the next node in the list.
Linked lists are often used because of their efficient insertion and deletion. They can be used to implement stacks, queues, and other abstract data types.


## Operations

### Time and space complexity

![Time Complexity](./operations.png)

![Time Complexity](./abc.png)


## When to use

- Use Array for fixed size data or data that needs more search / traversal / indexing than insertion deletion, need random access to a particular element
- Use Dynamic Arrays (Array List), when you want the best of Arrays and do not want to have restriction on size. Note the allocation will double everytime the border of initial allocation is passed. 
- Use Lists for large number of elements, size of list is big or is changing, adding and removing operation is performed more frequently than traversal or search 


## Pros and Cons

### Pros

Linked lists offer some important advantages over other linear data structures. Unlike arrays, they are a dynamic data structure, resizable at run-time. Also, the insertion and deletion operations are efficient and easily implemented.

### Cons

However, linked lists do have some drawbacks. Unlike arrays, linked lists aren't fast at finding the n^\text{th}n 
th
  item. To find a node at position nn, you have to start the search at the first node in the linked list, following the path of references nn times. Also, because linked lists are inherently sequential in the forward direction, operations like backward traversal--visiting every node starting from the end and ending in the front--is especially cumbersome.

Additionally, linked lists use more storage than the array due to their property of referencing the next node in the linked list.

Finally, unlike an array whose values are all stored in contiguous memory, a linked list's nodes are at arbitrary, possibly far apart locations in memory. This means that the CPU can't effectively cache the contents of a linked list nearly as well as an array resulting in poor performance. This is the main reason why ring buffers are used to implement queues instead of linked lists in high-performance applications where middle insertion and deletion functionality isn't needed (e.g. network drivers).


## Alternates

Doubly Linked List

Circular Linked List


## Resources
- https://brilliant.org/wiki/linked-lists/
