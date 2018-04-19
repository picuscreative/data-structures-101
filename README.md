# General purposes data structures

## Linked Lists
* small amount of data, not predictable
* used when data is frequently inserted and deleted
* searching is slow
* the insertion order matters when searching

## Arrays
* searching and deletion are slow
* delete is slow because an average of half the items must be moved to fill in the newly vacated cell
* fast access if index is known
* Ordered Array: small amount of data, predictable, search faster than insertion
* Unordered Array: small amount of data, predictable, insertion faster than search

## Binary Search Trees
* first choice when arrays and linked lists seems slow for solving the problem
* large amount of data, key distribution is random
* searching, insertion and deletion can be slow (in worst case)
* unbalanced trees reduce the performance

## Balanced Trees
* large amount of data, key distribution is not random
* complex and always balanced
* quick search, insertion and deletion whether the input data is ordered or not
* red-black trees (most used), 2-3-4 trees, AVL trees, splay trees, 2-3 trees
* sometimes a hash table may be a better choice than a balanced tree

## Hash tables
* large amount of data, fast search and insertion
* fastest data storage structure
* not sensitive to the order in which data is inserted
* simple than balanced trees
* if ordered traversal is necessary, a binary search tree is a better choice

## Summary (time complexity)

| Data Structure | Search | Insertion | Deletion | Traversal |
|---|---|---|---|---|
| Array | O(N)  |  O(1) end of array |  O(N) | - |
| Ordered Array | O(logN) binary search  |  O(N) | O(N)  |  O(N) |
| Linked List | O(N)  |  O(1) | O(N)  | - |
| Ordered Linked List | O(N)  | O(N)  |  O(N) | O(N)  |
| Binary tree (average) | O(logN)  |  O(logN) | O(logN)  |  O(N) |
| Binary tree (worst case) | O(N)  | O(N)  | O(N)  |  O(N) |
| Balanced tree (average and worst case) |  O(logN) |  O(logN) | O(logN)  |  O(N) |
| Hash table | O(1)  |  O(1) | O(1)  | - |

# Special purposes data structures
* Stacks, queues, and priority queues are Abstract Data Types (ADTs) implemented by fundamental data structures as arrays, linked lists or heaps

## Stacks
* use only to access last data item inserted (LIFO)
* implemented as an array or a linked list
* linked lists are a better choice when the amount of data that the stack will contain can’t be predicted in advance
* linked lists are a better choice because items can be inserted and deleted quickly from the head

## Queues
* use only to access first data item inserted (FIFO)
* implemented as an array or a linked list
* situations in which queue wraps around requires additional logic for an array, and double-ended linked lists
* linked lists are a better choice when the amount of data that the queue will contain can’t be predicted in advance

## Priority Queues
* use only to access first data with the highest priority
* implemented as an ordered array or a heap
* heaps are a better choice for faster insertion and deletion

## Summary (time complexity)

| Data Structure | Insertion | Deletion |
|---|---|---|
| Stack | O(1)  |  O(1) |
| Queue | O(1)  |  O(1) |
| Priority Queue (ordered array) | O(N)  |  O(1) |
| Priority Queue (heap) | O(logN)  |  O(logN) |
