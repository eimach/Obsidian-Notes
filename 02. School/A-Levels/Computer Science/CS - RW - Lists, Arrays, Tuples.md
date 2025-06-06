---
title: CS - RW - Lists, Arrays, Tuples
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-02-20
tags: [A-Level, Computer-Science, Data-Structures, CS]
type: Lesson Note
---

Links: [[Computer Science MOC]], [[CS - RW - Data Structures]]
Tags: #CS 
> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}


# List
- A list is like a normal list in Python.
- Can:
	- take multiple types (non-homogenous)
	- change size (dynamic)
	- change contents (mutable)
# 1-Dimensional Array
- An array is a finite, ordered collection of items of the same type (homogenous)
	- Size remains the same (static) --> *e.g. int listExample[30]*
	- Contents can be changed (mutable)
- **Arrays are stored contiguously in memory**
## Evaluation
- **Why might a dynamic data structure be used over a static?**
	- Dynamic will be useful as may not know how much space is needed to perform whatever task or don't know how much data is going to be stored in the list, such as a website database
- **Why might a static data structure be used over a dynamic data structure?**
	- Static might be used for something such as a map in a game which would have a set size or for when you know how much data you want to 
## Static Vs Dynamic

| Static                                                                                             | Dynamic                                                                                               |
| -------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| Useful if we know amount of items stored in advance                                                | Useful if we do not know the amount of items stored in advance                                        |
| Limited on how we can interact with it; we can populate, replace items (if mutable) and read items | As programmers, we can insert and remove items, in addition to the functions we can perform on a list |
| We know at time of definition how much space in storage it will hold                               | Not known how much space in storage it will hold; if it gets too large, can lead to overflow errors   |
# 2-Dimensional Array
- Are the same as a matrix
- Can be represented as:
	- `2D = [[1,2,3,4],[5,6,7,8],[9,10,11,12]]`
![[Pasted image 20250325162045.png]]
- Can access by doing `array[i][j]`
	- 6 would be `arrary[1][1]`
## Applications
- Used for Matrices and Mathematical Operations, Grid-Based Games, Image Processing
# 3-Dimensional Array
- Are like cubes and contain rows, columns and layers
	- Are like an array of 2D arrays where each layer represents a 2D matrix
- Can be represented as 3D =  ![[Pasted image 20250325162421.png]]
## Python Implementation
```python
# 3D array: 2 layers, 3 rows, 4 columns
array = [
    [  # Layer 1
        [1, 2, 3, 4],
        [5, 6, 7, 8],
        [9, 10, 11, 12]
    ],
    [  # Layer 2
        [13, 14, 15, 16],
        [17, 18, 19, 20],
        [21, 22, 23, 24]
    ]
]

# Accessing elements
print(array[0][1][2])  # Output: 7
print(array[1][2][3])  # Output: 24

```
## Applications
- Are used in 3D Graphics and Image Processing, Game Development, Storing Frames in Videos
# Tuple
- A tuple is a static, ordered collection of items that can be of different types (non-homogenous)
	- Static and Immutable - Size cannot change and Data cannot be changed