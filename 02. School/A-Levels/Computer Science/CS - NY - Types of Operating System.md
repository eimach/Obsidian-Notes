---
title: CS - NY - Types of Operating System
category: A-Level
subject: Computer Science
topic: Systems Software and Applications Generation
date: 2025-02-28
tags:
  - A-Level
  - Computer-Science
  - CS
  - Systems-Software-Applications-Generation
type: Lesson Note
---

> [!NOTE] Context/Summary
> Operating systems can be distributed across multiple computers (DOS), embedded into systems (home appliances), multi-tasked, multi-user, real-time. 
# Distributed Operating Systems
- A Distributed OS can coordinate the processing of a single job across multiple computers ![[Pasted image 20250228102721.png]]
- A program can be run by the user that uses data or resources from any other computer
	- Can include processor time, memory, I/O facilities
- The distribution of tasks is coordinated by the OS passing instructions between computers
- The user can access more computational power with the *illusion* of working with a single processor
	- There is no need for training or writing programs differently
	- ***BUT*** the programmer has no control over the task distribution due to this being handled by the OS
# Multi-Tasking System
- A single processor can appear to do more than one task simultaneously by scheduling processor time -> [[CS - NY - Functions of an Operation System|Processor Scheduling]]
## Multi-User, Multi-Tasking System
- Some systems use a very powerful computer called a mainframe
	- In Universities or Large Businesses
- Lots of users with their own terminals access the mainframe's CPU and each gets a time slice
- Each terminal (computer) is also running multiple processes
## Mobile Operating Systems
- A smartphone is a computer with a multi-tasking OS
	- e.g. iOS can run notes, calculator and other apps at the same time
- Mobile OS are linked to specific hardware
- A low-level proprietary OS is used for handling the hardware and special features
- Meanwhile, the main OS handles the user interface and running applications
# Open-Source Operating Systems
- Android is an open-source OS based on Linux and owned by Google
	- It is used by all major device manufacturers
	- Allows for major customisation
- A device manufacturer can fine-tune the OS to suit their devices and add additional features or user interfaces to enhance the user experience
	- Android is the basis of OxygenOS, LineageOS, OneUI
	- These can be major selling points
# Embedded Operating Systems
- Many home devices have an OS which can run simple programs
	- For example, washing machines, smart kettles, smart fridges.
## Household Devices
- The embedded OS has minimal features
- Application programs are held in ROM
- There is a limited amount of RAM
- The UI is simple and minimal
# Real-Time Operating Systems
- Some OSes *must* operate in real-time
	- Must respond extremely quickly to inputs
	- May need to cope with many inputs simultaneously
- Real-Time OSes are usually seen in *safety-critical* environments
- If a hardware component fails, the OS must have a *failsafe* to detect this and respond appropriately
- There is **Hardware Redundancy** -> crucial components are duplicated in the case that one fails
## Case Study - Therac-25
- 1980s radiation therapy machine with a real-time operating system
- Patients were treated for cancer through exposure to targeted beams of radiation
- Programming errors meant the machine responded incorrectly to certain real-time inputs
- Several people died as a result of accidentally being hit by massive radiation overdoses
# BIOS
- **Basic Input Output System** is stored in ROM
- BIOS boots the computer at start-up
	- Initialises and tests hardware
	- Loads the OS into RAM
# Device Drivers
- Drivers are programs that provides an interface for the OS to interact with a device
- Drivers are hardware *dependent* and OS *specific*
	- Drivers are needed to allow the OS to control hardware devices, from speaks to graphics cards
- The OS does not need to know the specifics of the hardware to be able to interact with it as generic drivers can be used ![[Pasted image 20250310144542.png]]
# Virtual Machines
- Software used to emulate a machine
- Can be used for running one OS inside another to emulate different hardware
- A virtual machine can execute intermediate code
	- e.g. a Java VM executes Java byte code
	- The MAME VM can emulate the hardware of old arcade machines so that their games can be played on a modern PC
# Related Notes
[[Computer Science MOC]]
[[CS - NY - Systems Software and Applications Generation]]
