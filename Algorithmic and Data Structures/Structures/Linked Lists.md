#Structure

A linked list is a continuous list of nodes where a node is a block structure housing the node value and a pointer (or memory) addres to the next node. Each node from the head node has a **next** pointer that keeps the address of the next node till it gets to the last node, which points to nothing.

![[Structures_LinkedList.png]]

## Types of Linked Lists

There are three types of linked lists:

1. Single-linked list
2. Doubly linked list
3. Circular Linked list

You can derive other linked lists from the bacis ones, e.g., circular doubly linked lists. 

### Single-linked list

You are tasked with building a tool to retrive documents connected to each other but stored at random memory locations, You are puzzled as to what data structured to use to fit this use case, as arrays store documents sequentially. The good news is that you can use the singly linked list for this tasks.

A singly linked list is defined by its node. A singly linked list node has a value and the next pointer. The diagram below is an example of singly linked list

![[Structures_LinkedList.png]]
A linked list with 4 nodes.  Each node points to another node. The last node always points to NULL, exceprt for circular Linked lists.


### Doubly linked list

You are tasked with implementing a new feature in a multiplayer board game (chess, checkers, tic-tac-toe, etc.) that enables a user to go back to their previous move. To implement this feature, you will likely to use a doubly linked list data structure.

A doubly linked list has two node pointers - one pointer pointing to the previous node and the other pointing to the next node.

Here is a graphical representation:

![[Structures_DoublyLinkedList.png]]
A doubly linked list representation. Each node keeps a pointer to the previous and next node.

### Circular Linked lists

Circular linked lists are singly linked lists except that their last node points to the first node as apposed to None. As a result, the circular linked list does not have a tail node.
Circular linked lists are commonly used to manage computing resources

![[Structures_CircularLinkedList.png]]
The circular linked list's last node's next pointer set to the first node is address



















