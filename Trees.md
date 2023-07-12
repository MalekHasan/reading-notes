# Trees
Trees are hierarchical structures composed of nodes connected by edges.Trees are used to represent hierarchical relationships or to organize data in a specific order. They provide efficient search, insertion, and deletion operations, making them useful for various applications such as organizing file systems, implementing search algorithms, representing hierarchical data, and more.

## Common Terminology

- ***Node*** - A Tree node is a component which may contain its own values, and references to other nodes
- ***Root*** - The root is the node at the beginning of the tree
- **K** - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
- ***Left*** - A reference to one child node, in a binary tree
- ***Right*** - A reference to the other child node, in a binary tree
- ***Edge*** - The edge in a tree is the link between a parent and child node
- ***Leaf*** - A leaf is a node that does not have any children
- ***Height*** - The height of a tree is the number of edges from the root to the furthest leaf


![Tree](./img//BinaryTree1.png)

## Types of Trees
1. Binary Tree: A binary tree is a type of tree in which each node has at most two children, referred to as the left child and the right child. The structure of a binary tree resembles a branching structure, similar to a family tree.

2. Binary Search Tree (BST): A binary search tree is a type of binary tree that follows a specific ordering property. For any node in the tree, the values in its left subtree are smaller, and the values in its right subtree are greater. This ordering property allows for efficient searching, insertion, and deletion operations.

3. K-ary Tree: A k-ary tree is a generalization of binary trees, where each node can have up to k children. It accommodates a higher branching factor and can be used to represent hierarchical relationships with more than two child nodes.

