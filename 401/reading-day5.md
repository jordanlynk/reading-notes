# Linked Lists

- A linked list is a sequence of Nodes (individual items/links) that are connected to each other. The most defining feature of a LL is that each node is a reference to the next in the link.
- **There are two types of linked list** *Singly*: (refers to the number of references a node has) & *Doubly*: (refers to there being 2 references within the node)
- *Next*: the property within a node that references to you guessed it, the next node.
- *Head*: reference type to the first node in a linked list.
- *Current*: the current node currently being looked at. 
- Biggest differences between arrays and linked lists: arrays are *static data structures*:(an organization or collection of data in memory that is fixed in size) while linked lists are *dynamic data structures*:( size of the structure is not fixed and can be modified during the operations performed on it).
- "A node only knows about what data it contains, and who its neighbor is"

## Traversal
- When we transverse (or walking through to do something with the data) we won't need a foreach or for loop. Instead we use the *Next* value to get us to where the reference is pointing. While walking through our data, the *Current* node is the most helpful.
