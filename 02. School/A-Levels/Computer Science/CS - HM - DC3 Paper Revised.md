---
title: CS - HM - DC3 Paper Revised
category: A-Level
subject: Computer Science
topic: Revision
date: 2025-03-04
tags: [A-Level, Computer-Science, CS]
type: Lesson Revision
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}

# Q1b
![[Pasted image 20250304091750.png]]
# Q1c
![[Pasted image 20250304091833.png]]
# Q3a
![[Pasted image 20250304092020.png]]
If question has many marks, the marks will be generous
``` python
def toBinary(val):
	binary = ""
	while val != 0:
		rem = val % 2 -> gives remainder
		val = val // 2 -> integer divides val
		binary = str(rem) + binary
	return binary
```
# Q3b
![[Pasted image 20250304093110.png]]
When it says "main program", **don't** define a function.
```python
num = int(input("Enter a number between 1 and 255"))
while num < 1 or num > 255:
	num = int(input("Enter a number between 1 and 255"))
binary = toBinary(num)
print(binary)
```
# Q6
```python
class video:
	def __init__(self, name)
		self.__name = name
		self.__number_of_views = 0
		self.__star_rating = 3
```
# Q7
## 9 Marker Structure
AO1 Knowledge - 4
	Application - 2
	Evaluation - 3
## 12 Marker Structure
AO1 Knowledge - 4
AO2 Application - 3
AO3 Evaluation - 5
## Question (12)
![[Pasted image 20250304094816.png]]
AO1 - Define OOP/Procedural, Encapsulation, Inheritance, Polymorphism
AO2 - Inheritance (in context of video games), Encapsulation (in context of video games), Polymorphism (in context of video games)
AO3 - Benefits/Drawbacks
	Why OOP
	List benefits and Drawbacks
Plan you Essay and Structure
Can lose marks when saying:
	Inaccurate statements
## Re-Attempt
Object-Oriented Programming is a programming method that allows involves the use of objects (classes) which contain variables called attributes and functions called methods. Encapsulation is an OOP technique that involves bundling attributes and methods and controlling whether they can be accessed through public or private functions. Inheritance is a technique of creating Child classes from a Parent Class which takes the exact same attributes and methods as the Parent Class. Polymorphism is an OOP technique which allows child classes to inherit a parent class's attributes and methods but change them to whatever needed.

In the context of a video game, Inheritance is useful as it would provide an easier way to creating entities such as weapons in an RPG as many child classes which represent different types of weapons could inherit base attributes from a parent "weapon" class. Polymorphism is useful in video games as it has child classes inherit (e.g. a goblin child class from a monster parent class) attributes and methods from a parent but change certain attributes or methods to suit its use case such as having different types of enemies. Polymorphism is useful in a game as it would prevent players from accidentally being able to change certain attributes and methods of a class such as the weapon or enemies and allows control over what class's attributes and methods can be modified.

For video games, OOP has a benefit of being able to work in teams during development as each member of a team can work on a separate class which would be difficult to achieve in procedural programming due to lack of classes. Another benefit of OOP is that it reduces code repetition which reduces the amount of code a computer has to execute which could lead to better optimisation and it also makes working in the codebase easier for developers. A drawback of OOP is that it can take a long amount of time to setup which could possibly hinder an inexperienced developer's work capacity.
# Q8c
**Procedure** means there is *no* return statement
![[Pasted image 20250304101050.png]]![[Pasted image 20250304101032.png]]
```python
def salesAnalysis():
	file = openRead("sales.txt")
	lines = file.readlines()
	days = 0
	sum = 0
	for line in lines:
		days += 1
		sum += float(line)
	file.close()
	print(days)
	print(sum/days) -> prints average
	print(sum) -> prints total sales
```
# Related Notes 
[[Computer Science MOC]]
