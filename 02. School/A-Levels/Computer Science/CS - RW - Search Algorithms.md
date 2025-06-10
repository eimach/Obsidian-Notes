---
title: CS - RW - Search Algorithms
category: A-Level
subject: Computer Science
topic: Algorithms
date: 2025-03-21
tags: [A-Level, CS, Computer-Science, Algorithms]
type: Lesson Note
---
# Linear Search
- A searching *algorithm* that checks each element in an *unordered array* sequentially
- Pseudocode for a **Linear Search** would be:
```function linearSearch(arr, item)
	for a in arr:
		if a != item
			return False
```
## Time Complexity of Linear Search
For a linear search, it would $O(n)$

# Binary Search
- A searching *algorithm* that checks for elements in a *ordered array* and checks by halving the array
- Pseudocode for a **Binary Search** in a *recursive* way would be:
```	function binarySearch(arr, item):
	left = 0
	right = arr.length() - 1
	if right >= left:
		mid = left + (right - left) // 2
		if arr[mid] == item
			return mid
		elif arr[mid] > item:
			return binarySearch(arr, left, mid-1, right)
		else: 
			return binarySearch(arr, mid + 1, right, item)
	else:
		return False
```
- Python Code for a **Binary Search** in an *iterative* way would be:
```
def binarySearch(arr, low, high, x):
    while low <= high:
        mid = low + (high - low) // 2
        if arr[mid] == x:
            return mid
        elif arr[mid] < x:
            low = mid + 1
        else:
            high = mid - 1
    return -1
```
## Time Complexity of Binary Search
- For a binary search, it would be $O(\log_{2}(n))$

# Dijkstra's Algorithm
- Purpose is to find the shortest path from a start note to all other nodes in a *weighted* graph -> [[CS - RW - Graphs|Graphs]] 
## Examples

| Node | Shortest Distance from A | Previous Node |
| ---- | ------------------------ | ------------- |
| A    | 0                        |               |
| B    | 3                        | A             |
| C    | 3                        | D             |
| D    | 1                        | A             |
| E    | 2                        | D             |
| F    | 5                        | E             |
| G    | 5                        | E             |

# A* Algorithm

# Time Complexity
- [[CS - RW - Time Complexity, Space Complexity & Big O Notation]]

# Related Notes
[[Computer Science MOC]]
[[CS - RW - Search Algorithms]]
[[CS - RW - Time Complexity, Space Complexity & Big O Notation]]