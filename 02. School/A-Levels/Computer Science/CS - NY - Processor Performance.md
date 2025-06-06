---
title: CS - NY - Processor Performance
category: A-Level
subject: Computer Science
topic: Components of a Computer and Their Uses
date: 2025-02-20
tags: [A-Level, Computer-Science, Computer-Components-Uses, CS]
type: Lesson Note
---

Links: [[Computer Science MOC]], [[CS - NY - Components of a Computer and Their Uses]]
Tags: #CS 
# Notes
## Words
- Memory is divided up in equal units called words
	- Word length is usually 8, 16, 32 or 64 bits
- Each word has a separate memory address

| Address  | Data or Instruction |
| -------- | ------------------- |
| 00000000 | 01101001            |
| 00000001 | 01101100            |
| 00000010 |                     |
| 00000011 | 10011111            |
## Address Bus
- The width of the address bus determines the *maximum* possible memory addresses of the system
- With an 8-bit Address Bus, the maximum number is 256  or 2<sup>8</sup>
- Average PCs have a memory capacity of 4GB which is 2<sup>32</sup> bytes
	- Therefore, it must have a 32-bit address bus
## Data Bus
- The data bus is bi-directional as data can be sent both ways along the bus
	- The width of the Data Bus is defined by the number of wires or lines it contains
- If the data bus is the same width as a computer word, data can be transferred to and from memory in a single operation
## Instruction Format
- Assembly language is very closely related to machine code
- The architecture of a computer, including word size and width of the address bus, determine the format of a machine code instruction for a particular type of processor
### Machine Code Instruction
![[Pasted image 20250121145215.png]]
## Performance Factors
- The main factors affecting processor performance are:
	- Clock Speed
	- Core Count
	- Type and Amount of Cache Memory
- The Fetch-Execute cycle is triggered by the clock pulses of the system clock
- The *faster* the clock speed, the *faster* a computer can fetch, decode and execute instructions
	- The clock can change state many billions of times per second
	- A 4GHz processor would tick 4 billion times per second
### System Clock
- A series of regular ON/OFF signals are used to synchronise the operations of the processor components
	- Actions are usually carried out on the rising edge
	- Actions each take a fixed number of cycles to complete ![[Pasted image 20250121150517.png]]
### Core Count
- Many computers today have multiple cores i.e.
	- A dual-core computer has 2 processors linked together in the same integrated circuit
	- A quad-core computer has 4 linked processors
- Each core is theoretically able to process a different instruction at the same time with its own Fetch-Execute Cycle
	- This makes a quad-core *2* or *4* times faster than a single-core
	- However, the software may not always be able to take full advantage of all four processors
### Parallel Processing
- Using several processor cores working at the same time is known as *Concurrent* or *Parallel Processing*
	- In systems designed for Parallel Processing, each core can work concurrently on different parts of the same task
	- Since instructions are processed sequentially, this is not always possible
### Cache Memory
- Cache is a small amount of superfast (*but expensive*) memory that stores data and instructions that have recently been used by the processor
	- Level 2 Cache is larger but *not as fast* as Level 1 Cache
	- Both types are held on the processor chip
![[Pasted image 20250121151059.png]]
- L1 Cache Memory is split into *Instruction Cache* and *Data Cache*, so that data and instructions can be fetch simultaneously
- The more Cache Memory a computer has, the more likely it is that it will not have to fetch the next instruction or data from RAM, as it will already have been loaded into the *superfast* Cache Memory from which it can be retrieved much more quickly
### Pipelining
- This is a technique used to improve performance, for example by overlapping stages in the Fetch-Execute Cycle, or by breaking down the stages in an arithmetic instruction
	- An instruction enters the pipeline, and as soon as one stage has been completed, another instruction enters the pipeline
	- A third instruction then enters before either of the others is completed
![[Pasted image 20250121151513.png]]
![[Pasted image 20250121151608.png]]
