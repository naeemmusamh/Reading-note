# Stacks and Queues

## What is a Stack????

A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

there is two concept the slack follow :

1. first in last out (FILO)

the first item added in the stack will be the last item popped out of the stack.

2. last in first out (lifo)

the last item added to the stack will be the first item popped out of the stack.

## What is Common terminology for a stack ???

1. Push :

is a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.

When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.

ALGORITHM push(value)
   node = new Node(value)
   node.next <-- Top
   top <-- Node

2. Pop :

Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.

ALGORITHM pop()
   Node temp <-- top
   top <-- top.next
   temp.next <-- null
   return temp.value

3. Peek :

conducting a peek, you will only be inspecting the top Node of the stack.

ALGORITHM peek()
   return top.value

4. IsEmpty :

Here is the pseudo code for isEmpty

ALGORITHM isEmpty()
return top = NULL

