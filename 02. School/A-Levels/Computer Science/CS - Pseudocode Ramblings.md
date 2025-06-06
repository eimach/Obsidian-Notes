Links: [[Computer Science MOC]]
Tags: #CS 
## Question:
Lesson: Exam Practice
**<span style="background:rgba(74, 82, 199, 0.2)">The function getIndex takes 2 parameters, an array and an item and should return the index of the first instance of the given item in the array. If the item is not in the array, it should return “Item is not in array”.</span>**
### Pseudocode Attempt:
function getIndex(array, item):
	search array for item
	if item is found in array
		end search
		return index of *item*
	else:
		return "Item is not in array"
### Walkden's Answer:
function getIndex(arr, item)
	for i in (o, length(getIndex)) do
		if arr[i] == item then
			return i
		end if
	end for
	return "Item is not in Array"
## Question:
Lesson: Exam Practice
<span style="background:rgba(5, 117, 197, 0.2)">The function add takes 3 parameters. A list, an item to be added to the list and the index it should be inserted at. It should return the new list with the item added. For example:</span>
<span style="background:rgba(5, 117, 197, 0.2)">add([“Albatross”, “Chicken”, “Dove”], “Buzzard”, 1) should return</span>
<span style="background:rgba(5, 117, 197, 0.2)">[“Albatross”, “Buzzard”, “Chicken”, “Dove”]</span>
### Pseudocode Attempt:
*not even done bru*
### Walkden's Answer:
function add(list, item, index)
	for i in (index.length(getIndex) -1) do
			list[i+1] = list[i]
	end for
	list[index] = item
	return list

## Question:
Writing pseudocode of methods for Pop, Peek, IsEmpty, IsFull
Lesson: [[CS - RW - Stacks]]

### Push
```
procedure push(item)
	if isFull then
		print("Stack is full")
	else:
		Head = Head + 1
		stack[Head] = item
	endif
```
### Pop
Attempt
```
procedure pop(item)
	if isEmpty then
		print("Stack is empty")
	else:			
		Head = Head - 1
		stack[Head] = item
	endif
```
Solution
```
procedure pop(item)
	if isEmpty then
		print("Stack is empty")
	else:			
		item = stack[Head]
		Head = Head - 1
		return item
	endif
endfunction
```
### Peek
```
procedure peek(stack)
	if isEmpty then
		print("The stack is empty")
	else
		return stack[Head]
	
```
### Is Empty
```
procedure isEmpty(stack)
	if Head
		return False
	else:
		return True
	endif
```
### Is Full
Attempt
```
procedure isFull(stack)
	if maxSize
		return True
	else:
		retrun False
	endif
```
Solution
```
procedure isFull()
```
## Queues - [[CS - RW - Queues]] 
Write pseudocode for the following functions:
	isFull, isEmpty, enQueue, deQueue, traverse
	*Variables: "Queue", "maxSize", "Head", "Tail" are global*
	"India" is Tail & "Golf" is Head

|     | "Golf" | "Hotel" | "India" |     |     |
| --- | ------ | ------- | ------- | --- | --- |

### isFull
```
function isFull(queue)
	if Head == maxSize - 1 and Tail == maxSize then:
		return True
	else:
		return False
	endif
endfunction

```
### isEmpty
```
function isEmpty(queue)
	if Head and Tail then:
		return False
	else:
		return True
	endif
endfunction
```
#### Solution
```
function isEmpty():
	if Head > Tail then
		return True
	else
		return False
	endif
endfunction
```
### enQueue - not finished - solution only
```
function enQueue(queue)
```
### deQueue - not finished - solution only
### traverse - not finished - solution only
```
procedure traverse():
	if isEmpty then
		print ("The Queue is Empty")
```
## Circular Queues - [[CS - RW - Queues]] 
Write pseudocode for the following functions:
	isFull, isEmpty, enQueue, deQueue, traverse
	*Variables: "Queue", "maxSize", "Head", "Tail" are global*
	"Lima" is Tail & "Hotel" is Head

| "Lima" | "Golf" | "Hotel" | "India" | "Juliet" | "Kilo" |
| ------ | ------ | ------- | ------- | -------- | ------ |

### isFull
```
function isFull()
	if maxSize == Tail + 1 mod maxSize
		return True
	else
		return False
	endif
endfunction

```
### isEmpty
```
function isEmpty()
	if Head > Tail mod maxSize then:
		return True
	else:
		return True
	endif
endfunction
```
### enQueue 
```
function enQueue(item):
	if isFull then
		print("The queue is full")
	else
		Tail = (Tail + 1) mod maxSize
		queue[Tail] = item
	endif
endfunction
```
### deQueue 
```
function deQueue():  
	if IsEmpty then  
		print("The queue is empty")  
	else  
		item = stack[Head]  
		Head = (Head + 1) mod maxSize  
		return item  
	endif  
endfunction
```
### traverse
```
procedure traverse():
	if isEmpty then
		print ("The Queue is Empty")
	else
		for i in range(head, ((tail + 1) mod maxSize))
			print(Queue[i])
		endfor
	endif
endprocedure
```