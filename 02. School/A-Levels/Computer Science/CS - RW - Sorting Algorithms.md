---
title: CS - RW - Sorting Algorithms
category: A-Level
subject: Computer Science
topic: Algorithms
date: 2025-05-12
tags: [A-Level, Algorithms, CS, Computer-Science]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# Insertion Sort
- For every item in the array, **insert** it into the correct position relative to everything before it
- Steps are:
	1) Start with the Second Item
	2) **Insert** it into the correct position in the array
	3) Move onto the next item
	4) Repeat until the whole list is sorted
- Demonstration: https://youtu.be/8oJS1BMKE64
- Time Complexity = $O(n$) in the best case scenario and $O(n^2)$

# Bubble Sort
- Iterate through data, swapping any adjacent values in the wrong order; leads to larger items rising to the top
- Steps are:
	1) Iterate through the array
	2) If the current item is larger than the next one, swap the two items
	3) Repeat until the end of the array is reached
	4) If the end has been reached without any swaps occurring, end the function
	5) Otherwise, iterate through the array again
- Demonstration: https://www.youtube.com/watch?v=Cq7SMsQBEUw
- Time Complexity = $O(n^2)$ 

# Merge Sort
- "*Divide and Conquer*" - keep splitting the array in half, until it is completely divided, then **merge** them back together *in order*
- Steps are:
	1) Split array in half
	2) Continue to split the left half of the array
	3) Repeat until left with an array of length 1
	4) Merge the arrays back together in order
	5) Repeat for the right half of the array ![[Pasted image 20250520134853.png]]
- Time Complexity = $O(n\log n)$ for Best Case *and* Worst Case
- Is a *Recursive* algorithm
- Demonstration

# Quick Sort
- Choose a "pivot" and split array to items above and below and pivot; Repeat until list is sorted
- Steps:
	1) Choose a "pivot"
	2) Split the array into items above and below the pivot
	3) Repeat for every generated array
	4) End when all arrays are of length **1**
	5) Combine the arrays from left to right ![[Pasted image 20250602113658.png]]
- Time Complexity: Worst Case = $O(n^2)$. Best Case = $O(n\log n)$ 
- Good Choice for Pivot?
- Why not always choose best pivot?
# Related Notes
[[CS - RW - Algorithms]]
[[CS - RW - Time Complexity, Space Complexity & Big O Notation]]