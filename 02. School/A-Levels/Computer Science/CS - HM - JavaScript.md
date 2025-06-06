---
title: CS - HM - JavaScript
category: A-Level
subject: Computer Science
topic: Web Technologies
date: 2025-02-20
tags: [A-Level, Computer-Science, Web-Technologies, CS]
type: Lesson Note
---

Links: [[Computer Science MOC]]
Related: [[CS - HM - HTML & CSS]]

> [!NOTE] Context/Summary
> This lesson is on JavaScript and Syntax

# Standard Conventions
- Uses Zero-Based Indexing
- When declaring variables, it is common to end the line with a semicolon
	- `let character = "Character";`
- Camel Casing is the standard for naming variables
	- `character; secondCharacter; secondCharacterAgain;`
- **Truthy** values are values which are evaluated as *True* when evaluated as a Boolean; most values in JavaScript are **truthy**
- **Falsy** values are considered *False* when evaluated as a Boolean;
	- Includes: `false`, `0`, `""`, `null`, `undefined`, `NaN`
# Syntax
- `let` - declares a variable and allows for it to be reassigned. When re-declaring variables  `let` does not need to be used
	- `let variable = 1; variable = 2`
- `const` - declares a variable that will remain constant and can *not* be reassigned 
- `console.log()` - prints x to console (same as print() in python)
- `first = 1; second = 2; second = first;` - can assign variables to other variables so `second` now is  the same as `first`
- `let arr = []` - declares `arr` as an array (same as lists in python)
- `console.log(arr[0])` - would print to the console the first item in `arr`
- `arr[1] = 25` - changes the indexed item to 25
- `.push(element)` - adds an element to the end of an array and returns the new length of the array
	- `rows.push("element")`
- `.pop()` - removes the last element of an array and returns the element
	- `rows.pop()`
## For Loops
- Basic Syntax of a For Loop:
```js
for (iterator; condition; iteration) {
  logic;
}
```
- Basic Syntax of a For...or Loop:
```js
for (const value of iterable) {
}
```
- This type of For Loop iterates over each item in an iterable object and temporarily assigns it to a variable
## Functions
```javascript
function name(parameters) {
}
```
## While Loops
- Let a piece of code run over and over again until the condition is no longer true
```js
while (condition) {
	logic;
}
```
## IF Statements
- Allows a block of code to be run *only* if a condition is met.
```js
if (condition) {
logic if condition conditon is met
} else if (condition2) {
logic if condition 2 is met
} else {
logic run if condition and condition 2 are not met
}
```