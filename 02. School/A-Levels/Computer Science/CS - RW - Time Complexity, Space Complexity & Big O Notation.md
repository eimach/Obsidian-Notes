---
title: CS - RW - Time Complexity, Space Complexity & Big O Notation
category: A-Level
subject: Computer Science
topic: Algorithms
date: 2025-03-25
tags: [A-Level, Computer-Science, CS, Algorithms]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}

# Time Complexity
- Default base for $\log()$ is **Base 2**
- $n$ is the size of the input data
- $O(1)$ is Constant Time - Regardless of the size of the input, it will take the same amount of time
-  $O(n)$ is Linear Time - The time increase is proportional to the *size* of the input
- $O(n^2)$ is Polynomial Time - The time increase is proportional to the *square* of the size of the input
- $O(2^n)$ is Exponential Time - Each item added to the input will *double* the time
- $O(\log(n))$ is Logarithmic Time - As the input data *increases*, the time increases at a *slower* rate
- $O(n!)$ is Factorial Time - Is ridiculously slow. As the size increases, the time is $n!$ 
![[Pasted image 20250325134324.png]]


## Simple Principles
- If there is a loop in the code -> $O(n)$
- If there is a loop nested in a loop -> $O({n^2})$
- If there is a loop nested in a loop nested in a loop... etc -> $O(n^3)$
- If there is a loop then another loop *not nested* -> $O(2n)$ but turns into $O(n)$
- If statements and normal statements such as variable assignments -> $O(1)$
- If splitting data in half -> $O(\log n)$

# Space Complexity
- Is the same as **Time Complexity**, except that we are interested in space rather than time
	- As the data input increases, does the required memory increase?
# Related Notes
[[Computer Science MOC]]
[[CS - RW - Algorithms]]
