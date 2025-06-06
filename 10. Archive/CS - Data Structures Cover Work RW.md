# Q1: 
### i) State the meaning of the term static
The term static means that the size of the data structure can not be changed/has a fixed size
### ii) State one type of data structure that is always considered to be static
A 1-Dimensional Array
### iii) State the meaning of the term dynamic
The term dynamic means that the size of the data structure can be changed
### iv) Give one disadvantage of using a dynamic data structure
One disadvantage of a dynamic data structure can be that it requires more memory usage and processing power
# Q2
### a)
Identifier: Board
Number of dimensions: 3x15
Most appropriate data type: 3-D Array
### b)
PROCEDURE ClearDisplay
	FOR Row = 1 TO 3
		FOR Column = 1 to 15
			Board(Row, Column) = " "
		NEXT Column
	NEXT ROW
END PROCEDURE
# Q4
### a)

| "2+3" | "1+4" | "3-1" | "10/2" | "3+6" |     |     |     |
| ----- | ----- | ----- | ------ | ----- | --- | --- | --- |

### i)

| "2+3" | "1+4" | "3-1" | "10/2" | "3+6" | "6+1" |     |     |
| ----- | ----- | ----- | ------ | ----- | ----- | --- | --- |
### ii)
head = 0
tail = 5