
# Sets ADT

## Overview
- A set is a ADT that can store any number of unique values in any order you so wish.
- a set is an abstract data type that can store unique values, without any particular order. It is a computer implementation of the mathematical concept of a finite set. Unlike most other collection types, rather than retrieving a specific element from a set, one typically tests a value for membership in a set.

Types
- Statis Sets: Some set data structures are designed for static or frozen sets that do not change after they are constructed. Static sets allow only query operations on their elements — such as checking whether a given value is in the set, or enumerating the values in some arbitrary order. 
- Other variants, called dynamic or mutable sets, allow also the insertion and deletion of elements from the set.
- A multiset is a special kind of set in which an element can figure several times.
- Disjoint Sets: stores a collection of disjoint (non-overlapping) sets

ADT implemented using
- List : Inefficient
- Trees
- Tries
- Hashtables

## Operations

![Time Complexity](./operations.png)

![Time Complexity](./abc.png)


## When to Use

## Pros and Cons

#### Pros:


#### Cons:


### Variation

#### MultiSet:

A generalization of the notion of a set is that of a multiset or bag, which is similar to a set but allows repeated ("equal") values (duplicates). This is used in two distinct senses: either equal values are considered identical, and are simply counted, or equal values are considered equivalent, and are stored as distinct items. For example, given a list of people (by name) and ages (in years), one could construct a multiset of ages, which simply counts the number of people of a given age. Alternatively, one can construct a multiset of people, where two people are considered equivalent if their ages are the same (but may be different people and have different names), in which case each pair (name, age) must be stored, and selecting on a given age gives all the people of a given age.

#### Disjoint Set:

https://en.wikipedia.org/wiki/Disjoint-set_data_structure

## Resources


