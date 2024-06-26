
# [Linked List](#linkedlist)
A linked list is a data structure that consists of a group of nodes where each node contains a data value and a reference (or link) to the next node in the list.

## [Table of Contents](#table-of-contents)

- [Linked List](#linkedlist)
  - [Table of Contents](#table-of-contents)
  - [Example](#example)
  - [Time complexities of some basic Linked List operations](#time-complexities-of-some-basic-linked-list-operations)
  - [Types of Linked List](#types-of-linked-list)
    - [Singly Linked List](#singly-linked-list)
    - [Doubly Linked List](#doubly-linked-list)
    - [Circular Linked List](#circular-linked-list)
    - [Circular Linked List](#circular-linked-list)
  - [Linked List Use Cases](#linked-list-use-cases)

## [Example](#example)
```
let list = [4,3,1,0,14,6];
```

| Memory Location | Value |
|-----------------|-------|
| 1000             | 4     |
| 1001             | 1008  |
| 1002             | 1     |
| 1003             | 1004  |
| 1004             | 0     |
| 1005             | 1006  |
| 1006             | 14    |
| 1007             | 1010  |
| 1008             | 3     |
| 1009             | 1002  |
| 1010             | 6     |
| 1011             | 1000  |

Accessing an element in a linked list is done by traversing the list and finding the element at the correct index.
```
index 0 value is 4 with memory location 1000 and pointer to next node 1008
index 1 value is 3 with memory location 1008 and pointer to next node 1002
index 2 value is 1 with memory location 1002 and pointer to next node 1004
index 3 value is 0 with memory location 1004 and pointer to next node 1006
index 4 value is 14 with memory location 1006 and pointer to next node 1010
index 5 value is 6 with memory location 1010 and pointer to first node 1000
```

<p align="center">
  <img src="images/LinkedList.png?raw=true" alt="Linked List Image"/>
</p>


## [Time complexities of some basic Linked List operations](#time-complexities-of-some-basic-linked-list-operations)

| Operation | Time Complexity |
|-----------------|-------|
| Accesing an element             | O(N)     |
| Searching an element           | O(N)     |
| Inserting an element             | O(1)     |
| Deleting an element             | O(1)     |

## [Types of Linked List](#types-of-linked-list)

### There are four types of Linked list

<p align="center">
  <img src="images/linkedListTypes.png?raw=true" alt="Linked List Image"/>
</p>

 + Singly linked list
 + Doubly linked list
 + Circular linked list
 + Circular doubly linked list


### [Singly Linked List](#singly-linked-list)


<p align="center">
  <img src="images/singlyLinkedList.png?raw=true" alt="Linked List Image"/>
</p>



There are many applications for singly linked lists. One common application is to store a list of items that need to be processed in order. For example, a singly linked list can be used to store a list of tasks that need to be completed, with the head node representing the first task to be completed and the tail node representing the last task to be completed.

Singly linked lists are also often used in algorithms that need to process a list of items in reverse order. For example, the popular sorting algorithm quicksort uses a singly linked list to store the list of items that need to be sorted. By processing the list in reverse order, quicksort can sort the list more efficiently.

### [Doubly Linked List](#doubly-linked-list)



<p align="center">
  <img src="images/doublyLinkedList.png?raw=true" alt="Linked List Image"/>
</p>



A doubly linked list is a bi-directional linked list. So, you can traverse it in both directions. Unlike singly linked lists, its nodes contain one extra pointer called the previous pointer. This pointer points to the previous node.

A doubly linked list of singly linked lists is a data structure that consists of a set of singly linked lists (SLLs), each of which is doubly linked. It is used to store data in a way that allows for fast insertion and deletion of elements.

Each SLL is made up of two parts: a head and a tail. The head of each SLL contains a pointer to the first element in the list, and the tail contains a pointer to the last element.

It is advantageous over other data structures because it allows for quick insertion and deletion of elements. Additionally, it is easy to implement and can be used in a variety of applications.

### [Circular Linked List](#circular-linked-list)


<p align="center">
  <img src="images/circularLinkedList.png?raw=true" alt="Linked List Image"/>
</p>

A circular Linked list is a unidirectional linked list. So, you can traverse it in only one direction. But this type of linked list has its last node pointing to the head node. So while traversing, you need to be careful and stop traversing when you revisit the head node.

### [Circular Doubly Linked List](#circular-doubly-linked-list)


<p align="center">
  <img src="images/CircularDoublyLinkedList.png?raw=true" alt="Linked List Image"/>
</p>


A circular doubly linked list is a mixture of a doubly linked list and a circular linked list. Like the doubly linked list, it has an extra pointer called the previous pointer, and similar to the circular linked list, its last node points at the head node. This type of linked list is the bi-directional list. So, you can traverse it in both directions.

## [Linked List Use Cases](#linked-list-use-cases)

- Dynamic Size:
  - When the size of the collection is not known in advance or changes frequently, linked lists provide a dynamic and flexible structure. You can easily add or remove elements without the need for resizing or reallocation.

- Efficient Insertion and Deletion:
  - Linked lists excel in scenarios where frequent insertion and deletion operations are expected. Adding or removing elements in the middle of a linked list involves updating references, making these operations more efficient compared to arrays.

- Memory Efficiency:
  - Linked lists can be more memory-efficient than arrays when dealing with dynamic sizes. Each element occupies its own node, and memory is allocated only as needed. This can reduce memory wastage compared to arrays, where a fixed-size block is allocated.

- Dynamic Data Structures:
  - Linked lists are often used as the foundation for implementing more complex dynamic data structures, such as stacks, queues, and hash tables.

- No Preallocation:
  - Unlike arrays, linked lists don't require preallocation of memory for a fixed size. This makes them suitable for situations where the exact size is not known in advance.

- Ease of Insertion/Deletion in the Middle:
  - If you frequently need to insert or delete elements in the middle of the collection, linked lists provide a more straightforward solution. You can adjust references without the need to shift elements.

- No Contiguous Memory Requirement:
  - Linked lists do not require contiguous memory blocks, making them advantageous in situations where memory is fragmented or when elements need to be scattered throughout memory.

- Implementation of Data Structures:
  - Linked lists are fundamental for implementing more advanced data structures like trees and graphs. In these structures, nodes are interconnected using references, and linked lists provide a natural way to represent these connections.