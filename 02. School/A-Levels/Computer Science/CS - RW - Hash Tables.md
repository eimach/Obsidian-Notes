---
title: CS - RW - Hash Tables
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-03-11
tags: [A-Level, Computer-Science, CS, Data-Structures]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# What do Hash Tables Do?
- If you were to have a list of numbers such as [78, 55, 19, 29, 98, 27, 47] and wanted to see if a number (e.g. 47) was in the list without searching the list or building a binary search tree:
	- Create an empty of a size (e.g. 11) and label each space in the list with the numbers (e.g. 0 - 10)
	- For each value in the list, do the *number* **mod** *array size* and then place it in that spot in the array
		- e.g. 78 mod 11 = 1
	- To check for values, do the *number* **mod** *array size* and see what is returned
	- If you run into a **collision**, where a number already has a value in place of where it should be, put it in the next available spot
		- e.g. 34 mod 11 = 1 but 1 has 78 so put 34 in 2
- Typically used in *Databases* or *Dictionaries*

## Example
Size 15, [43, 96, 28, 23, 100, 79, 18, 1, 70, 57]

| 0   | 1   | 2   | 3   | 4   | 5   | 6   | 7   | 8   | 9   | 10  | 11  | 12  | 13  | 14  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|     | 1   |     | 18  | 79  |     | 96  |     | 23  |     | 100 | 70  | 57  | 43  | 28  |

# Alternative Hashing Algorithms
## Folding
- For longer numbers, split the number into equal parts, sum the parts, then take that *result* **mod** the *hash table size*
	- e.g. putting the phone number 01543 677896 into a table of size 100
	- 01 + 54 + 36 + 77 + 89 + 6 = 263
	- 263 mod 100 = 63
### Folding Example

| Number | Hash Table Location |
| ------ | ------------------- |
| 123456 | 2                   |
| 238464 | 71                  |
| 188947 | 54                  |
| 276084 | 72                  |

## Hashing a String
- We can hash a string by using the ASCII code for each character
	- e.g. in a hast table of 11, the string "CAB" would be done like:
		- 67 + 65 + 66 = 198
		- 198 mod 11 = 0
# Hashing Functions
- A good hashing function does the following:
	- Can be calculated very quickly
	- Reduces the likelihood of collisions
	- Does not use too much memory
# Solving the Collision Problem (Rehashing)
- Possible solutions:
	- Place it in the next position in the array
	- Place it "*x*" spaces away (Skip Factor)
	- Use another array in that position and store the value in there; would need to do a linear search to find it
	- Use a linked list in that position and add the value there

# Hash Tables v. Binary Search Trees

| Hash Table                                                             | Binary Search Tree                                                                              |
| ---------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Less Memory Efficient - Need more spaces in the table than data values | Stores as many spaces as data values - 1 space per data value                                   |
| Worst Case Scenario: Have to search through every item                 | Performance depends on balance of tree - Worst Case Scenario: Have to search through every item |
| Best Case Scenario: 1 step to find your value (no collisions)          | Best Case Scenario: log2(n)                                                                     |
| Better for checking existence                                          | Better for searching in a range *or* finding nearest number                                     |
 
# Related Notes
[[Computer Science MOC]]
[[CS - RW - Data Structures]]