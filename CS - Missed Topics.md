**FIGURE OUT WHERE TO GO LATER**

# CISC vs RISC
- CISC - Complex Instruction Set Computer
	- CISC has lots of commands -> Shorter Code - *Benefit*
	- Requires more complex hardware - **Drawback**
- RISC - Reduced Instruction Set Computer
	- Each command takes one *FDE* (Fetch, Decode Execute) cycle
	- RISC has a small number of commands -> When put together, creates more commands -> Longer Code - **Drawback**
	- Only requires simple hardware - *Benefit*
	- More efficient - *Benefit*

# Von Neumann vs Harvard Architecture
- Von Neumann - **shared** memory holds data *and* instructions
	- Can only access memory for one thing at a time -> Data **or** Instructions
- Harvard - **separate** memory for data and instructions
	- Can access memory for data and instructions at the same time

# Multicore and Parallel Systems
- Single Core Processors can do **Task Switching** -> Makes it look like its multi-tasking in parallel
	- Task Switching - Switching between tasks very quickly
- Multi-Core Processors can **Parallel Processing** -> Running multiple tasks at the same time
- Not always possible to process things in parallel -> Some tasks must be done consecutively
- More Cores != More Processing Power --> Cores must communicate, eventually diminishing returns
## What affects a Processors Speed?
- Clock Speed -> Higher Clock Speed can do more FDE cycles
- Increase Cache Size -> RAM processes are slow --> Increasing Cache Size means that less data needs to be offloaded to RAM as frequently
- Increase Core Count

# Software Methodologies
- Methodologies are ways of making software
## Waterfall
- Split into Analysis, Design, Development, Testing, Evaluation
- Each step is done one at a time
- Useful when there is *No Risk* and *Clear Requirements*
## Spiral
- Split into Analysis, Design, Development, Testing, Evaluation -> Same as Waterfall
- Done in a spiral
- Useful for reducing *risk* and developing prototypes
## Rapid Application Development (RAD)
- Move as fast as possible to produce prototypes
- Useful for focusing on *speed* and producing prototypes
## Extreme Programming
-  Main Focus is on  the *code* *quality*
- Pair Programming is used
## Agile
- Same as **RAD** but focused on releasing versions of the final product
- Work fast to develop an initial version of the product that can be released and updated upon receiving feedback

# Related Notes
[[Computer Science MOC]]