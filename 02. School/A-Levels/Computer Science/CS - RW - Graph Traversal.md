---
title: CS - RW - Graph Traversal
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-02-20
tags: [A-Level, Computer-Science, Data-Structures, CS]
type: Lesson Note
---

Links: [[Computer Science MOC]], [[CS - RW - Data Structures]]
Tags: #CS 
Related: [[CS - RW - Graphs]]
Useful Links: [DFS & BFS Maze](https://www.youtube.com/watch?v=zMy5MwQWwss), [Reachability Problem Simulation](https://www.cs.usfca.edu/~galles/visualization/DFS.html)

> [!NOTE] Context/Summary
> SHOW HOW THESE ARE IMPLEMENTED
# Notes
## Breadth First Search (*BFS*)
- From the starting vertex, visit all vertices 1 edge away. Then visit all vertices 2 edges away, then all vertices 3 edges away
	- Implemented using a [[CS - RW - Queues|Queue]]
- Returns shortest route in an unweighted graph
	![[Pasted image 20250210114410.png]]
### Python Implementation
```python
list = [A, C, B, F, D, K, J, G, H, E]
queue = [A!, C!, B!, F!, D!, K!, J!, G!, H!, E!]
```
## Depth First Search (*DFS*)
- Keep going until you find an end point
- When there is a choice of edges, any can be picked as long as you are consistent
	- Implemented using a [[CS - RW - Stacks|Stack]]
- Cons: Runs the risk of falling into a loop if not implemented properly
	- Can be remedied by checking if node is already in list
	![[Pasted image 20250210114727.png]]
### Python Implementation
``` python
list = [A, C, F, J, H, D, G, E, B, K]
```
Stack: 

| D   |     |
| --- | --- |
| H   |     |
| J   |     |
| F   | K   |
| C   | B   |
| A   |     |
## Reachability Problem
- DFS and BFS are useful for this
- [Reachability Problem Simulation](https://www.cs.usfca.edu/~galles/visualization/DFS.html)

DFS:
A, B, E, F, H, C, G, D
BFS:
A, B, D, C, G, E, F, H