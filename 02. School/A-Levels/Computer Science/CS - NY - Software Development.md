---
title: CS - NY - Software Development
category: A-Level
subject: Computer Science
topic: Systems Analysis Methods
date: 2025-04-25
tags:
  - A-Level
  - CS
  - Computer-Science
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}
# What Are the Types of Software?
- There are two categories:
	- *Applications Software* and *Systems Software* -> [[CS - NY - Systems Software and Applications Generation]], [[CS - NY - Nature of Applications]]

# Software Development Stages
- **Software Development** from the *initial idea* to the *final product*, follows 5 stages: ![[Pasted image 20250425092628.png]]
## Analysis Stage
- A *systems analyst* gathers information about what the current system does, *if it is present*, and what the new system needs to do
- They may do this by:
	- **Interviewing** who will use the software
	- Use **questionnaires** to get information from large groups of people
	- **Observe** how the current system works
	- Look at existing *documentation*
- Eventually, the systems analyst will produce a document, usually called "*System Specification*" or "*User Requirements*" which defines **what** the system will do, but not how to do it
	- This is used to create the design and to evaluate the finished product
## Design Stage
- Software design will include:
	- A description of the data: *data type*, *format*, *validations*
	- Database Design, *if appropriate*
	- Input Screens
	- Output Screens and Reports
	- How data will be processed
	- How software will be tested
## Implementation Stage
- Implementation includes:
	- Coding and Testing the Software
	- Writing User and Technical Documentation
	- Installing the Software for the User
### Black Box Testing
- Is carried out independently of the code used in the program
- Looks at the program specification and creates a set of test data that covers all the inputs, outputs and program functions
### White Box Testing
- This type of testing depends on the *Code Logic*
- Tests are devised which test each path through the code *at least once*
### Alpha Testing
- Carried out by the software developer's in-house team and by the user
- Can reveal errors or omissions in the definition of the system requirements
- The user may discover that the system does not do exactly what they wanted
### Beta Testing
- Used when commercial software is being developed
- The software is given to a number of potential users, who agree to use the software and report any faults
- Helpful as real users may try and to things that were **not anticipated** by the developer
## Evaluation Stage
- Checking *if it all works*
- The user now needs to test every aspect of the software to make sure it does what it is supposed to do
- It will be evaluated against the original specification document
- This stage can also be called **Acceptance Testing**
## Maintenance Stage
- There are three types of ***Maintenance***:
	- **Corrective**: Bugs will usually be found when the software is put into action, no matter how thoroughly it was tested
	- **Adaptive**: Over time, user requirements will change and the software will have to be adapted to meet new needs
	- **Perfective**: Even if the software works well, there may be way of making it even better -> faster, easier to use, more functionality, more efficient
- Then the Cycle begins again.

# Development Methodologies
- There main **methodologies** are *Waterfall*, *Spiral*, *Agile*, *Extreme*, *Rapid Application Development*
## Waterfall 
- Each stage in the lifecycle model is completed and documented before the next is begun
- This results in the customer not seeing the end product until it is completed
- Any change to be made often means the project has to be started again
- **Advantages of the Waterfall Methodology**:
	- *Simple* to *Understand* and *Use*
	- Each stage is *Separate* and *Self-Contained* with well defined outcomes and written documentation
	- This makes the project *relatively straightforward* to *manage*
	- The model works well for *smaller projects* where *requirements are very well understood*
- **Disadvantages of the Waterfall Methodology**:
	- There is *not* much *user involvement* after the **Analysis** stage, where the Specification document is agreed
	- No working software is produced until late in the cycle
	- The user is presented with the finished product and if it is not what was required, generally too late to make changes
- **When to Use?**:
	- Clear and Fixed Requirements
	- No Ambiguous Requirements
	- Well-Understood Technology
	- Short Projects
## Spiral
- The four basic steps, *Analysis*, *Design*, *Implementation* and *Evaluation* are followed
- The software project passes through these phases *repeatedly*
- Each successive loop round the spiral generates a new, more refined **prototype** until the software meets all the requirements ![[Pasted image 20250425101601.png]]
- **Advantages of Spiral Methodology**:
	- Well-defined steps make the project easy to manage
	- Software is produced at an early stage so problems and issues can be identified early
	- The user gives feedback on each prototype and any required changes can be made early in the process
	- Added functionality can be added during the process
	- The end result is more likely to be what the user wants
- **Disadvantages of Spiral Methodology**:
	- Developing prototypes, getting feedback, refining prototypes is time-consuming so the finished product takes longer to develop
	- A system is more costly to develop because of the time involved
	- Not suitable for smaller projects
- **When to Use?**:
## Agile
- Software is developed in *rapid incremental cycles*
- Each version builds on previous functionality
- Each version is thoroughly tested before release
- Good for small, time-critical projects
- Limited planning is needed to get started![[Pasted image 20250425101542.png]]
- **Advantages of Agile Methodology**:
	- Rapid, continuous delivery of useful software leads to customer satisfaction
	- Customers, developers and testers constantly interact with one another
	- Working software is delivered frequently, within weeks rather than months
	- Software is easily adapted to changing circumstances
	- Even late changes in requirements can be implemented
- **Disadvantages of Spiral Methodology**:
	- Lack of emphasis on necessary design and documentation
	- Project can fail to deliver if the customer is not clear about the desired final outcome
	- Not suitable for novice programmers - Experienced programmers capable of making good decisions are required
- **When to Use?**:
	- When new changes need to be implemented - small incremental changes can be made frequently and for little cost
	- In an expanding or developing business where users' needs are continuously changing and developing
## Extreme Programming
- A type of **Agile** software development
- Frequent releases of the software are made in short development cycles
- Intended to improve productivity and responsiveness to changing customer requirements
## Rapid Application Development (RAD)
- Workshops and Focus Groups gather requirements rather than using a formal document
- Prototyping is used to continually refine the system in response to user feedback
- Each part of the system is produced within a strict time limit - maybe not perfect but good enough
- Software components are reused whenever possible
# Related Notes
[[Computer Science MOC]]
[[CS - NY - Systems Analysis Methods]]