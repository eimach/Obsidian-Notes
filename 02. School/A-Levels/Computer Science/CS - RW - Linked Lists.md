---
title: CS - RW - Linked Lists
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-03-12
tags: [A-Level, Computer-Science, CS, Data-Structures]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# What Are Linked Lists?
- Linked Lists are a *non-contiguous* data structure where data is stored in nodes and connected through pointers
- The nodes contain both the data in that node as well as the pointer to the next node in the list ![[Pasted image 20250312165636.png]]
- Linked Lists are *Dynamic* as they can grow and shrink if/when needed.
- They are efficient at inserting and deleting elements as data is not held in order, so elements don't need to be shifted unlike in arrays
- **However**, they are slower as each node must traversed one by one and no node can be directly accessed through an index
# Types of Linked Lists
- There are 3 types of Linked Lists:
	1. Singly Linked Lists
	2. Doubly Linked Lists
	3. Circular Linked Lists
## Singly Linked Lists
- These are the standard linked lists where nodes are one-directional and only point to the next node in the list
- Used for Dynamic Memory Allocation, Undo Functionality, Polynomial Representation
## Doubly Linked Lists
- These are linked lists where nodes are bi-directional and point to the node behind and in-front
- Used for File Systems, Undo/Redo, Back and Forward Navigation in Web Browsers
## Circular Linked List
- These are singly linked lists where the last node points back to the first node, creating a continuous loop
- Used for Round-Robin Scheduling, Music/Video Playlists, Buffer Management
## Doubly Circular Linked List
- These are doubly linked lists where the last node points back to the first node, creating a continuous loop and each node points to the previous node
# Related Notes
[[Computer Science MOC]]
[[CS - RW - Data Structures]]