---
title: CS - NY - Processor Components
category: A-Level
subject: Computer Science
topic: Components of a Computer and Their Uses
date: 2025-02-20
tags: [A-Level, Computer-Science, Computer-Components-Uses]
type: Lesson Note
---

Links: [[Computer Science MOC]], [[CS - NY - Components of a Computer and Their Uses]]
# Notes
## Central Processing Unit
- The processor (aka the CPU) has a number of different components, each with their own role to perform:
	- Control Unit
	- Buses
	- Arithmetic Logic Unit (ALU)
	- Dedicated Registers
### Control Unit
- The part of the processor that coordinates the activity of all other components
	- Control signals are sent along the control bus between the control unit and the other components of the computer
		**Control Signals** include:
		- Memory Read: causes data from the addressed location in RAM to be placed on the data bus
		- Memory Write: causes data on the data bus to be written into the addressed location in RAM
		- Bus Request: indicates that a device is requesting use of the data bus
		- Bus Grant: indicates that the CPU has granted access to the data bus
		- Clock: used to synchronise operations
### Buses
- Buses in a computer consist of a series of connectors that transfer signals between components
- The *<span style="background:rgba(5, 117, 197, 0.2)">system bus</span>* consists of three separate buses carrying control signals, addresses and data.
- ![[Pasted image 20250107152738.png]]
### Arithmetic-Logic Unit (*ALU*)
- Is the problem solving part of the processor
	- Performs arithmetic, logical and shift operations on data
	- Arithmetic Operations: Add, Subtract, Multiply, Divide
	- Logical Operations: AND, OR, NOT, XOR 
	- Shift Operations: Move bits to the *Left* or *Right* within a register
	- ![[Pasted image 20250120144217.png]]
 
### The Accumulator
- Rather than writing working data back to ‘slow’ memory, processors have several locations of super-fast memory called registers that are used to temporarily store results
- The processor is then able to immediately access and re-use these results in subsequent calculations, e.g. Add 2 + 3 + 4
### Dedicated Registers
- Program Counter (PC): Holds the memory address of the next instruction to be executed
- Current Instruction Register (CIR): holds the current instruction -> split into *opcode* and *operand*
- Memory Address Register (MAR): holds the address in memory where the processor is required to fetch or store data from or to
- Memory Data Register (MDR): temporarily holds data moving between the processor and main memory
- Accumulator: to hold intermediate results of an instruction

## Fetch-Execute Cycle
- Processors operate in defined stages that are used to carry out program instructions
	- **Fetch, Decode, Execute**
- ### Fetch Stage
	1. The address of the next instruction is copied from the PC to the Memory Address Register (MAR)
	2. The instruction held at that address is copied to the Memory Data Register (MDR)
	3. Simultaneously, the contents of the Program Counter (PC) are incremented
	4. The contents of the MDR are copied to the Current Instruction Register (CIR)
- ### Decode
	5. The instruction held in the CIR is decoded
	6. It is split into operand and opcode to determine the type of instruction it is. Addition data, if required, is fetched from memory
	7. and passed to the accumulator
		- The opcode specifies the operation to be carried out
		- The operand holds either:
			- The address of the data to ben used which is then copied to the MAR, ***or***
			- The actual data to be operated on which is passed to the MDR
- ### Execute
	8. The instruction is executed and the result held in the accumulator or stored in memory 