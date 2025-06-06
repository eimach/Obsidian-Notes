---
title: CS - NY - Functions of an Operation System
category: A-Level
subject: Computer Science
topic: Systems Software and Applications Generation
date: 2025-02-24
tags: [A-Level, Computer-Science, CS, Systems-Software-Applications-Generation]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on the Functions and Purpose of an OS
> - The OS manages **memory allocation**, **CPU time** and *provides* a **UI**.
> - Memory can be allocated in **pages** or **segments**.
> - The CPU processes jobs according to a **scheduling algorithm**
> - The CPU can be *interrupted* if a job with a **higher priority** arrives.
> 

# What is an Operating System?
- Software is needed to manage communication with computer hardware
	- The Bootloader in ROM loads the OS into RAM when the computer is switched on
	- The OS manages the hardware and provides an interface for the user and the application software![[Pasted image 20250224145235.png]]
- The Functions the OS provides are:
	- User Interface
	- Memory Management
	- Interrupt Handling
	- Processor Scheduling
## User Interface
- The OS hides the complexity of the hardware from the user through a UI
	- For example, the frontend UI hides the commands running in the backend
## Memory Management
- Programs and their data need to be loaded into RAM
- The OS manages the allocation of RAM to the different program
- There may not be sufficient RAM for all desired processes to be *completely* loaded into RAM at once
### Paging
- Available memory is divided into *fixed-size* chunks called **Pages**
	- Each page has an address
	- A process loaded into RAM is allocated sufficient pages, but those pages may not be *contiguous* (next to each other) physically
![[Pasted image 20250224150459.png]]![[Pasted image 20250224150518.png]]![[Pasted image 20250224150533.png]]
![[Pasted image 20250224150608.png]]
### Segmentation
- Alternatively, memory is divided into segments which may be different lengths
- Segments can relate to parts of a programs
	- e.g. a function or subroutine may occupy a segment

|                       Similarities                       |                                     Differences                                      |
|:--------------------------------------------------------:|:------------------------------------------------------------------------------------:|
|  Both allow programs to run despite insufficient memory  |                     Pages are fixed size. Segments are variable                      |
|          Pages and Segments are stored on disk           | Pages are made to fit sections of memory. Segments are complete sections of programs |
| Pages and Segments are transferred into memory when need |           Pages are *physical* divisions. Segments are *logical* divisions           |

### Virtual Memory
- A computer has a fixed amount of RAM and the memory demanded will often exceed it
- A section of the HDD or SSD -> [[CS - NY - Storage Devices|Storage Devices]] can be designated as virtual memory
- Some pages of a current process will be stored in virtual memory until needed, which will then be swapped into RAM
- If many processes are running and the computer has insufficient RAM, *lots* of time is spent swapping pages in and out of virtual memory
	- This can *noticeably* slow down the computer -> Known as **Disk Thrashing**
## Interrupts
- It is vital that the CPU can be interrupted when necessary
- Interrupts can be sent to the CPU by software, hardware or the CPU's internal clock
	- e.g. I/O device sends an interrupt signal, Printer runs out of paper, An error occurs in a program, Scheduled interrupt from the internal clock, Power Failure
- The CPU check at the end of each clock cycle whether there are interrupts which need to be processed ![[Pasted image 20250225144425.png]]![[Pasted image 20250225144425.png]]
### Using the Stack
- When an interrupt is detected, the processor stops fetching instructions and instead pushes the current contents of its registers onto a stack ![[Pasted image 20250225145553.png]]
- The CPU uses an **Interrupt Service Routine** (***ISR***) to process the interrupt
	- When processing has finished, the values can be popped from the stack and reloaded into the CPU ![[Pasted image 20250225145810.png]]
### Interrupt Priority
- Interrupts have different priorities and will be processed in order of priority
- Interrupts can be interrupted if there is a new interrupt with a higher priority
- If a higher priority interrupt occurs whilst an interrupt is being processed, the original interrupt's registers will be pushed onto the stack as well  ![[Pasted image 20250225145112.png]]
- [[CS - RW - Stacks|Stacks]] are LIFO data structures so the last data to be pushed on will be the first to retrieved ![[Pasted image 20250225145226.png]]
## Processor Scheduling
- A single CPU can only process instructions for one application at a time
- The OS must schedule when each application can use the CPU
- This gives the illusion of *multi-tasking* - multiple applications appear to be running simultaneously
- There are multiple different Scheduling Algorithms which can be
	- **Pre-Emptive** and *Non* **Pre-Emptive**
### Aims of Scheduling
- To Provide an acceptable response time to all users
- To maximise the time the CPU is usefully engaged
- To ensure fairness on a multi-user system
### Round Robin (RR)
- Each job is allocated, *by a FIFO system*, a time slice during which it can use the CPU's resources
- If the job has been completed by the end of its time slice, the next job is allocated a time slice ![[Pasted image 20250225151158.png]]
- Works on a First Come, First Served basis
	- The first job to arrive is executed until it is completed
### Shortest Remaining Time (SRT)
- The time to completion is estimated as each new job arrives
- The job with the shortest remaining time to completion is executed -> means that a shorter *new* job can take over from the process
- **Pre-emptive**
### Shortest Job First (SJF)
- a.k.a. *shortest process next*
- As with *Shortest Remaining Time*, the total execution time of each job is estimated by the user
- The waiting job with the smallest total execution time is executed when the current job completes
### Multi-Level Feedback Queues (MLFQ)
- Multiple queues are created with different *priority* levels
- If a job uses too much CPU time, it is moved to a *lower* priority queue
- Processes can also be moved to a higher priority queue if they have waited a long time
# Related Notes
- [[Computer Science MOC]]
- [[CS - NY - Systems Software and Applications Generation]]
- [[CS - RW - Stacks]]