# Queue Data Structure

## Overview
A collection of items in which only the earliest added item may be accessed. Basic operations are add (to the tail) or enqueue and delete (from the head) or dequeue. Delete returns the item removed. Also known as "first-in, first-out" or FIFO.
- Abstract Data type, can be implemented with Array, LinkedList, Heap.. For priority Queue Binary heap gives best performance

[Types](https://www.hackerearth.com/practice/data-structures/queues/basics-of-queues/tutorial/)
- DeQue (Short for Double-Ended QUEue. A queue in which items can be added or deleted from both ends)
- [Priority Queue](https://xlinux.nist.gov/dads/HTML/priorityque.html)( An abstract data type to efficiently support finding the item with the highest priority across a series of operations. )
- [Calendar Queue](https://xlinux.nist.gov/dads/HTML/calendarQueue.html)(A fast priority queue implementation having N buckets each with width w, or covering w time.)
- Circular Queue : One of the benefits of the circular queue is that we can make use of the spaces in front of the queue. In a normal queue, once the queue becomes full, we cannot insert the next element even if there is a space in front of the queue. But using the circular queue, we can use the space to store new values.
- Binded Queue ( A queue limited to a fixed number of items.)

## Operations

![Time Complexity](./operations.png)
Enqueue: O(1)
Dequeue: O(1)
Size: O(1)

![Time Complexity](./abc.png)


## When to Use
- Serving requests on a single shared resource, like a printer, CPU task scheduling etc.
- In real life scenario, Call Center phone systems uses Queues to hold people calling them in an order, until a service representative is free.
- Handling of interrupts in real-time systems. The interrupts are handled in the same order as they arrive i.e First come first served.
- CPU scheduling, Disk Scheduling
- When data is transferred asynchronously between two processes.The queue is used for synchronization

## Pros and Cons

#### Pros:
Queues have the advantages of being able to handle multiple data types and they are both flexible and flexibility and fast. Moreover, queues can be of potentially infinite length compared with the use of fixed-length arrays.


#### Cons:
A major disadvantage of a classical queue is that a new element can only be inserted when all of the elements are deleted from the queue. Solution is to have a ciruclar queue


### Alternate
https://en.wikipedia.org/wiki/Circular_buffer


## Resources
