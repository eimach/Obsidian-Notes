---
title: CS - RW - Graphs
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-02-20
tags: [A-Level, Computer-Science, Data-Structures]
type: Lesson Note
---

> [!NOTE] Context/Summary
Graphs are a *Data Structure* used to represent complex, non-linear relationships
# Notes
## Keywords:
- Vertices/Nodes
- Edges/Arcs
- Undirected/Directed - Bidirectional or Unidirectional
- Weighted/Unweighted
- Dense/Sparse
## Definition of Graph
- A *Data Structure* used to represent complex, non-linear relationships
## Graphs
- Graphs consist of nodes/vertices connected by edges/arcs which may be Directed *or* Undirected and Weighted *or* Unweighted
- Graphs can be **Dense** which means that each *node* is connected to another *node* by an *edge*. They can also be **Sparse** which means that not every *node* is connected to another node by an *edge*
## Adjacency Matrix
- An Adjacency Matrix is a matrix used to represent a finite graph
- The elements of the matrix indicate whether node pairs are adjacent or not
	- 1 if Two Nodes are Directly connected. 0 if Two Nodes are not Directly connected
![[Pasted image 20250130120538.png]] 
- This Graph would have this Adjacency Matrix:

|       | **A**   | **B**   | **C**   | **D**   | **E**   | **F**   |
| ----- | --- | --- | --- | --- | --- | --- |
| **A** | 0   | 1   | 1   | 1   | 0   | 0   |
| **B** | 1   | 0   | 0   | 0   | 0   | 0   |
| **C** | 1   | 0   | 0   | 0   | 1   | 0   |
| **D** | 1   | 0   | 0   | 0   | 0   | 1   |
| **E** | 0   | 0   | 1   | 0   | 0   | 1   |
| **F** | 0   | 0   | 0   | 1   | 1   | 0   |
![[Pasted image 20250130120841.png]]
- In a *Weighted* Adjacency Matrix, the weight is stored in the matrix instead of **1** or **0**
- There are different conventions for what happens with unconnected nodes
	- Can leave unconnected graphs empty
	- Can place a 0 in the spot (*least used*)
	- Place an infinity symbol 
## Adjacency List
![[Pasted image 20250130121101.png]]
- In Python, these would be stored as a Dictionary:
 ``` python
adjList = {A:[B,C,D], B:[A], C:[A,E]} 
```
- For weighted graphs, the Adjacency List is represented differently
![[Pasted image 20250130121314.png]]
- In Python, it would be stored as a Dictionary within a Dictionary
```python
{E:{G:2}, C:7, N:3}, G:{C:4}}
```
