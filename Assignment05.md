# Read05

## Linked Lists

- A linked list is a linear data structure, in which the elements are not stored at contiguous memory locations. The elements in a linked list are linked using pointers as shown in the below image:

![](Linkedlist.png)

-  a linked list consists of nodes where each node contains a data field and a reference(link) to the next node in the list.

### Traversing a Linked List
A linked list is a linear data structure that needs to be traversed starting from the head node until the end of the list. Unlike arrays, where random access is possible, linked list requires access to its nodes through sequential traversal. Traversing a linked list is important in many applications. For example, we may want to print a list or search for a specific node in the list. Or we may want to perform an advanced operation on the list as we traverse the list. The algorithm for traversing a list is fairly trivial.

- Start with the head of the list. Access the content of the head node if it is not null.

- Then go to the next node(if exists) and access the node information

- Continue until no more nodes (that is, you have reached the last node)

###  Insert at the beginning
- Allocate memory for new node
- Store data
- Change next of new node to point to head
- Change head to point to recently created node
 

### Insert at the End
- Allocate memory for new node
- Store data
- Traverse to last node
- Change next of last node to recently created node

### Insert at the Middle
- Allocate memory and store data for new node
- Traverse to node just before the required position of new node
- Change next pointers to include new node in between

### Delete from a Linked List

#### Delete from beginning
- Point head to the second node

#### Delete from end
- Traverse to second last element
- Change its next pointer to null

#### Delete from middle
- Traverse to element before the element to be deleted
- Change next pointers to exclude the node from the chain
