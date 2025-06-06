---
title: CS - RW - Queues
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-02-20
tags: [A-Level, Computer-Science, Data-Structures, CS]
type: Lesson Note
---

Links: [[Computer Science MOC]], [[CS - RW - Data Structures]]
Tags: #CS 
Related: [[CS - RW - Lists, Arrays, Tuples]], [[CS - RW - 2D & 3D Arrays, Records, Linked Lists]], [[CS - RW - Stacks]], [[CS - Pseudocode Ramblings]]

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# Notes
- Queues are a First In, First Out (FIFO) data structure. This means that we remove from the front of the queue and add to the back of the queue
- Like in [[CS - RW - Stacks|Stacks]], we need a pointer to track where the front of the queue is (*Head*) so we know where to remove items from
- We also need a pointer to tell where the back of the queue (*Tail*) is so we know where to add items to.
- In some implementations, the tail will point to the next available space in the queue instead of the final value
	- May be referred to as the "Next Free Space" pointer
- Queues can be static or dynamic depending on whether they are implemented using a list or an array
## Queues Vs Stacks

| Queues                           | Stacks                    |
| -------------------------------- | ------------------------- |
| First In, First Out (FIFO)       | Last In, First Out (LIFO) |
| Uses two pointers, Head and Tail | Uses one pointer, Head    |
| Can be Static or Dynamic         | Can be Static or Dynamic  |
## Circular Queue
- In a Circular Queue, the head and tail pointers loop back around to the start (*if there is available space*)
