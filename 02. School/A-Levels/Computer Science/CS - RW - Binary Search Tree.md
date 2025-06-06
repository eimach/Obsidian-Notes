---
title: CS - RW - Binary Search Tree
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-03-03
tags: [A-Level, Data-Structures, Computer-Science, CS]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
>
# Binary Search Trees
- Graphs are the most flexible
- Binary Trees have at most *2* child nodes
- Binary Search Trees have the data added in a way that it allows for fast searching
- BSTs are useful if the data is sorted 
## Steps
1. Start at the root node
2. If the number is less than the root, go to the left. If the number is greater than the root, go to the right
3. Repeat until number or dead end
## Operations
### Removing a Node
-  If the node has no children, just simply remove it
- If the node has *one* child, replace the node with its child
- If the node is the root, find the successor (next number numerically or next letter alphabetically) and put everything to the left of the root to the left of the successor (new root) and everything to the right of the the root to the right of the successor
# Search Algorithm
- Inorder DFS will return nodes in alphabetical or numerical order -> [[CS - RW - Trees]]
# How to Store Binary Trees
- You can store a binary tree as an array of records, where each record stores the *data value*, *data value to the left* and the *data value to the right*
- If drawn, it is typically represented as a table
## Example
![[Pasted image 20250303121823.png]]

| Record  | Left | Data | Right |
| ------- | ---- | ---- | ----- |
| Tree[0] | 8    | 17   | 22    |
| Tree[1] | 4    | 8    | 12    |
| Tree[2] | 19   | 22   | 30    |
| Tree[3] | -1   | 4    | 5     |
| Tree[4] | -1   | 12   | 14    |
| Tree[5] | -1   | 19   | -1    |
| Tree[6] | 25   | 30   | -1    |
| Tree[7] | -1   | 5    | -1    |
| Tree[8] | -1   | 14   | -1    |
| Tree[9] | -1   | 25   | -1    |

# Related Notes
[[Computer Science MOC]]
[[CS - RW - Data Structures]]
[[CS - RW - Trees]]