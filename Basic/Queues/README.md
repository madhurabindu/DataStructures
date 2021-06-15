# Queue Data Structure

## Overview
A collection of items in which only the earliest added item may be accessed. Basic operations are add (to the tail) or enqueue and delete (from the head) or dequeue. Delete returns the item removed. Also known as "first-in, first-out" or FIFO.
- Abstract Dat type

Types
- DeQue (Short for Double-Ended QUEue. A queue in which items can be added or deleted from both ends)
- [Priority Queue](https://xlinux.nist.gov/dads/HTML/priorityque.html)( An abstract data type to efficiently support finding the item with the highest priority across a series of operations. )
- [Calendar Queue](https://xlinux.nist.gov/dads/HTML/calendarQueue.html)(A fast priority queue implementation having N buckets each with width w, or covering w time.)
- Circular Queue : One of the benefits of the circular queue is that we can make use of the spaces in front of the queue. In a normal queue, once the queue becomes full, we cannot insert the next element even if there is a space in front of the queue. But using the circular queue, we can use the space to store new values.
- Biunded Queue ( A queue limited to a fixed number of items.)

## Operations

![Time Complexity](./operations.png)

![Time Complexity](./abc.png)


## When to Use

## Pros and Cons

#### Pros:


#### Cons:


### Alternate
https://en.wikipedia.org/wiki/Circular_buffer


## Resources
