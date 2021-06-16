# Map ADT
Map is a ADT Also called Associative arrays, Symbol table or Dictionary

## Overview
- A Map is a Abstract data type, can be implemented with
  - Arrays (Vector, ArrayList)
 - Linked-list (O(n))
 - Binary search trees
 - Hash tables (O(1)) refer for details about hashing (http://www.bowdoin.edu/~ltoma/teaching/cs210/fall09/Slides/Maps.pdf)
- The ''key'' is an identifier for some kind of data, and the ''value'' is the content that is being identified or saved. 
- A Map is a type of fast key lookup data structure that offers a flexible means of indexing into its individual elements.
- Indices into the elements of a Map are called keys. These keys, along with the data values associated with them, are stored within the Map. 
- Each entry of a Map contains exactly one unique key and its corresponding value. 

## Operations

![Time Complexity](./mapimp.png)

![Time Complexity](./abc.png)


## When to Use
Need a fast lookup
In case of a sorted list (array), the worst case run-time complexity of a search operation is O(log n) when using the Binary Search algorithm.

Now the question is,

Can we further improve the efficiency of the search operation ?

The answer to that question is,

The efficiency of the search operation cannot be improved further as long as the search operation involves comparing values.

The Bin Sort Algorithm is the solution where the search operation efficiency can be improved to O(1) i.e. constant time. However, the Bin Sort algorithm has the following limitations:

Stores Only Numeric Values
Range For Storing The Numeric Value Should Be Known In Advance
All Values Should Be Unique
Wastage Of Space As The Values Are Stored Sparsely
The solution to the above listed limitations of the Bin Sort algorithm is a HashMap which is a HashTable implementation where the data is stored in Key-Value pairs. The Key and Value pair together is known as an Entity. All the keys should be unique.

A hash function is used to derive a bucket location where the element i.e. the value needs to be stored. The Key is passed as an input to the hash function which returns the bucket location. This improves the search efficiency by the O(1) i.e. constant time provided there is no collision (which is rarest of the rare case).

A collision is a situation where multiple keys are hashed to the same bucket location. Every HashMap implementation should implement a collision resolution strategy to store all those values whose keys are getting hashed at the same bucket location. Seperate Chaining with LinkedList, Seperate Chaining with Self Balancing Binary Search Trees, Open Addressing, etc…

Now the search operation efficiency is O(1+M/N) where O(1) is the constant time to reach the bucket using the hash function. M is the number of elements stored and N is the number of buckets available in the HashMap. M/N determines the load factor.

Along with collision resolution strategy, the HashMap should be rehashed everytime a load factor of the implementation is about to be reached. This helps in maintaining a balanced HashMap which keeps the search operation efficiency close to O(1). Generally, a load factor of 0.75 is defined to keep the HashMap balanced.


## Pros and Cons

#### Pros:
The major advantage of using a HashMap is to achieve close O(1) efficiency for search and delete operation. O(1) efficiency for add operation, meaning constant time


#### Cons:
The major disadvantage is the rehashing operation performed when the load factor is about to be reached as a rehashing operation is a costly operation in terms of run-time efficiency.
Implementation may not be thread safe
Complexity of hashing algorithm
Hashing algorithm might consume time
Additional space required for storing hash


### Alternate
- If you know your keys (what you're using to lookup your data) fall into a very narrow integer range, then an array (or preferably a vector) is ideal if all you care about is lookup. You can look up using a key in constant time with no fuss.
- If your key space becomes too large or is not an integer then Array can not be used
- A map lets you maintain reasonable lookup performance (O(log(n))), but only takes up 2 spots to store the memory
- Also key can be any type, not necessarly integer
- multimap is like map but allows the keys to be not unique
- unordered_map is a map that does not store items in order, but can provide better lookup performance if a good hash function is provided


## Resources


