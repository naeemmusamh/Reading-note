# Linked Lists

A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

There are two types of Linked List - Singly and Doubly. We will be implementing a Singly Linked List in this implementation.

1. Singly : 

 Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

2. Doubly :

 Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

Next =====>> This property contains the reference to the next node.

When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing. The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.

The best way to approach a traversal is through the use of a while() loop. This allows us to continually check that the Next node in the list is not null. If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash/end.

When traversing through a linked list, the Current variable will tell us where exactly in the linked list we are and will allow us to move/traverse forward until we hit the end.


A- Code

ALGORITHM Includes (value)

  Current <-- Head

  WHILE Current is not NULL
    IF Current.Value is equal to value
      return TRUE

    Current <-- Current.Next

  return FALSE

B- Algroithm

1. create Head and is always the first node in a Linked List.

2. We create a while loop. This loop will only run if the node that Current is pointing to is not null. 

3. checking if the value of the current node is equal to the value we are looking for.

4. If the Current node does not contain the value we are looking for, we then must move Current to the next node that is being referenced.

5. Once we hit the end, we know that we did not find the value and return true at any point, so the value is not in the LinkedList. We return false.