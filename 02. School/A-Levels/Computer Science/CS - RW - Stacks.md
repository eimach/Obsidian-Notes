---
title: CS - RW - Stacks
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-02-20
tags: [A-Level, Computer-Science, Data-Structures, CS]
type: Lesson Note
---

Links: [[Computer Science MOC]], [[CS - RW - Data Structures]]
Tags: #CS 
# Notes
## Stacks:
- In a stack, the items are added in a certain order and then removed in a certain order
- Specifically, when removing an item, we remove the top item (most recently added)
- If we were to remove an item from the stack, the top item would be removed.
	- `stack.pop()` would return "Delta" and remove it from the stack
	- Stacks are known as a "Last in, First Out" (LIFO) Data Structure
- We can also add items to a stack, the new item would be added at the top of the stack
	- `stack.push()` would return a new item such as "Echo" and put Echo on top of "Delta"

| Stack     |
| --------- |
| "Delta"   |
| "Charlie" |
| "Bravo"   |
| "Alpha"   |
- To keep track of stacks, we have a pointer called "Head" or "Top" which stores the index of the top of the stack
- May be known as the "Next Free Space" Pointer 
	- There are different conventions around using this pointer:
			Some may point the "Head" pointer to the top item or the spot above the top of the stack
- Stacks can be *Dynamic* or *Static* - depending on whether the stack is implemented as a list or an array
### Common Methods
- Push - add item to stack
- Pop - remove item from stack
- Peek - return top item of stack
- IsEmpty - return True if stack is empty, False if stack is not empty
- IsFull - return True if stack is full, False if stack is not full