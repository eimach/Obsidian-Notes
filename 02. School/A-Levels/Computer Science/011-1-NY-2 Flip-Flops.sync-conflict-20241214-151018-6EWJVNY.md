Links: [[Computer Science MOC]], [[CS - NY - Boolean Algebra]]
Tags: #CS 
# Notes
---
- A flip flop is an elemental sequential logic circuit that can store one bit and flip between two states, 0 and 1.
- A D-type Flip-Flop has one input (D) and two outputs (Q & NOT Q) + a clock signal
- The clock is another type of sequential circuit that changes state at regular time intervals.
	- It is needed to synchronise the change of state on flip flop circuits.
	- [[Drawing 2024-12-13 09.37.57.excalidraw]]
- ## D-Type Flip Flop as a Memory Unit
	- ![[Pasted image 20241213093726.png]]
	- Output Q only takes on a new value if the value at D has changed at the rising edge of a clock pulse
	- ![[Pasted image 20241213094159.png]]
	- D changes at times marked **A,B,C,E,F,G**
	- If D stays the same on the next clock pulse, the flip-flop retains current value, otherwise it flips.
	- Output Q = D on rising edges marked **J,K,L,M**
- ## Use of D-Type Flip-Flops
	- Creating registers and counters
	- For the intermediate storage needed during arithmetic operations
	- Static RAM is also created using D-Type Flip-Flops
		- *It is faster and more expensive than regular Dynamic RAM which must be periodically refreshed.*
		- Static RAM is typically used for cache memory. DRAM is used for main memory.


## Summary:

| Clock           | D               | Q(next) |
| --------------- | --------------- | ------- |
| Rising Edge     | 0               | 0       |
| Rising Edge     | 1               | 1       |
| Non-Rising Edge | X("Don't Care") | Q       |


