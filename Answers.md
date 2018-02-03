1. Stacks And Queues
 Stacks are a Last-In-First-Out(LIFO) data structure. Insertions are done in such a way that the most recently inserted items will be retrieved first. For example if we insert  4 -> 3 -> 8 in the order from left the right, when we retrieve from the stack at that state, 8 will the element returned, with the stack now having 3 -> 8.

 Queues are a First-In-First-Out (FIFO) data structure. Items are retrived in the order they are inserted.  If we insert 10 -> 12 -> 8 in the order from left to right,when retrieving an item 10 will be returned, with the stack now having 12 -> 8 as its elements.

 2. Retrieval Time Complexity
 A linked list has an 0(n), linear time for a retrival. Just Scan through the list by accessing the pointers to the next node.
 Hash tables can have a 0(c), constant time. With a well implemented hashing algorithm that avoids collisions and a table that resizes, key-value pairs should be well distributed amongst buckets, such that retrival is only the cost of calling a constant time hash function.
 Binary Search Trees can have 0(log n) logarithmic time complexity when retrieving elements. If the trees are inbalanced, ie. all nodes go along one branch, then BST retrieval will be 0(n).

 3. Hash tables can provide constant time retrieval, insertion and deletion, but most implementations don't provide methods for iteration or modification(splice,foreach,reduce,filter) of elements. If you only need to retrieval, insertion and deletion on large quanties of data, then the effiency of hash tables will be useful. If you to modify all your data or have needs to partition it, arrays can be more useful.