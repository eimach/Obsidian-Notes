---
title: CS - RW - Trees
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-02-25
tags: [A-Level, Computer-Science, Data-Structures]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# What Are Trees?
- A variation on a graph with a hierarchical structure with "*parent*" and "*child*" nodes
	- Feature *Roots* and *Leaves*
	- No Cycles
# Tree Traversal
- Trees use Depth First Searches to be traversed -> [[CS - RW - Graph Traversal]]
- There are 3 Types of DFS:
	- **Inorder** - Left, Root, Right
	- **Preorder** - Root, Left, Right
	- **Postorder** - Left, Right, Root
## Preorder DFS - *Root, Left, Right*
- Preorder Traversal is useful for copying the tree
- Go Left **FIRST** always
### Steps
1. Start at the root node
2. Follow the leftmost path until you reach a leaf
3. Backtrack and make a decision
### Example
![[Pasted image 20250225134831.png]]
- This would return [A,B,E,F,C,D,G,H,I,J]
## Inorder DFS - *Left, Root, Right*
- Useful for returning the order of Binary Search Tree
- Returns the tree as it reads from left to right
### Steps
1. Start from leftmost leaf
2. Go to parent node
3. Is there an unexplored child node?
	1. If yes, select the leftmost child node and find that child's leftmost leaf
4. Repeat until whole tree is traversed
### Example
![[Pasted image 20250225135243.png]]
- This would return [E,B,F,A,C,G,D,I,H,J]
## Postorder DFS - *Left, Right, Root*
- Useful for deleting the tree
- Start at the leaves and work inward
### Steps
1. Start from the leftmost leaf
2. Find the leaves from the sibling node
3. Work up the tree, starting from the leaves
4. Children should always be returned before parents
### Example
![[Pasted image 20250225140143.png]]
- This would return [E,F,B,C,G,I,J,H,D,A]
## Breadth First Search
- Useful for returning items in the tree in order of seniority
### Steps
1. Start with the root note
2. Visit its children
3. Then grandchildren
4. Then great grandchildren
5. Continue until all leaves are reached
### Example
![[Pasted image 20250225141015.png]]
- This would return [ABCDEFGHIJ]
## Example of All Traversal Methods
![[Pasted image 20250225141323.png]]
- BFS = [ABCDEFGHIKL]
- Preorder DFS = [ABEIJKFCDGHL]
- Inorder DFS = [IEJKBFACGDLH]
- Postorder DFS = [IJKEFBCGLHDA]
# Related Notes
[[Computer Science MOC]]
[[CS - RW - Data Structures]]
[[CS - RW - Graphs]]
[[CS - RW - Graph Traversal]]