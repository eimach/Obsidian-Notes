---
title: <% tp.file.title %>
category: A-Level
subject: Computer Science
topic: Data Structures
date: 2025-03-06
tags:
  - A-Level
  - Data-Structures
  - CS
  - Computer-Science
type: Lesson Note
---
> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# Inorder DFS Steps
- Inorder -> Left, Root, Right
	- Perform an inorder search on the Left subtree
	- Print the Root
	- Perform an inorder search on the right subtree
![[Pasted image 20250306115843.png]]![[Pasted image 20250306115902.png]]![[Pasted image 20250306120158.png]]![[Pasted image 20250306120232.png]]
- This returns [D,G,P,Q,S,T,W]
- Is an example of a **Recursive Algorithm** -> an algorithm which calls itself on smaller parts of the problem
## How to Program It?
``` 
Procedure InorderDFS(root):
	if root.left != -1 then
		InorderDFS(root.left)
	endif
	print(root.data)
	if root.right != -1 then
		Inorder DFS(root.right)
	endif
```
# Postorder DFS Code
- Left, Right, Root
```
Procedure PostorderDFS(root):
	if root.left != -1 then
		PostorderDFS(root.left)
	endif
	if root.right != -1 then
		PostorderDFS(root.right)
	endif
	print(root.data)
```
 
# Related Notes
[[Computer Science MOC]]
[[CS - RW - Data Structures]]
[[CS - RW - Trees]]
[[CS - RW - Binary Search Tree]]
