# Trees

- Root: the first/top node in the tree
- Left Child: Node that is positioned to the left of a root or node
- Right Child: same as left child, but to the right
- Edge: the link between parent and child node
- Leaf: does not contain any children
- Height: this is determined by the number of edges from the root to the very bottom node.
- **Binary Trees**: Restrict the number of children to two (left and right children). There is no specific order, nodes can be added into a binary tree if space allows for it. 
    - Strategy for adding a new node is to fill all "child" spots from the top down. 
    - In order to place a node in a specific spot, you need reference to both the new node to create and the parent node that the child is attached to.
- **Big O**: The Big O time complexity for inserting a new node is O(n). Searching for a specific node will also be O(n). 
- **Binary Search Tree**: a type of tree that does have some structure attached to it. All values that are smaller than the root are placed to the *left*, all values that are larger are placed to the *right*.
## Traversal:
- Allows us to serach for a node, print out the contents, etc
- Two types: *Depth First & Breadth First*
  - **Depth First**:
  - Prioritizes the depth (aka height) of the tree first. There are multiple ways to accomplish depth first traversal:
  - Pre-order: root >> left >> right. (Means that the root has to be looked at first)
  - In-order: left >> root >> right (Means we will output the root.value to the console)
  - Post-order: left >> right >> right 
  - **Recursion** is the most common way to traverse through a tree. We rely on call stack to navigate back up the tree.
  - **Breadth First**:
  - This method first traversal iterates through the tree by going through each level of the tree node-by-node.
  - Breadth first traversal uses a *queue* to traverse the width/breadth of a tree.
  - 
