# Trees

Common Terminology

1. Node ===> A Tree node is a component which may contain it’s own values, and references to other nodes.

2. Root ===> The root is the node at the beginning of the tree.

3. K ===> A number that specifies the maximum number of children any node may have in a k-ary tree.

4. Left ===> A reference to one child node, in a binary tree.

5. Right ===> A reference to the other child node, in a binary tree.

6. Edge ===> The edge in a tree is the link between a parent and child node.

7. Leaf ===> A leaf is a node that does not have any children.

8. Height ===> The height of a tree is the number of edges from the root to the furthest leaf.

![tree](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG)

## Traversals

An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:

1. Depth First :

Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, like :

A. Pre-order (root -> left -> right)

Pre-order means that the root has to be looked at first, and when we call preOrder for the first time, the root will be added to the call stack.

Next, we start reading our preOrder function’s code from top to bottom.

B. In-order (left -> root -> right)

C. Post-order (left -> right -> root)

The most common way to traverse through a tree is to use recursion.

2. Breadth First :

Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.