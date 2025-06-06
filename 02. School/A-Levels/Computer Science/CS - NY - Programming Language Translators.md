---
title: CS - NY - Programming Language Translators
category: A-Level
subject: Computer Science
topic: Systems Software and Applications Generation
date: 2025-03-14
tags: [A-Level, Computer-Science, CS, Systems-Software-Applications-Generation]
type: Lesson Note
---

> [!NOTE] Context/Summary
> This lesson is on {insert context or summary}

# Assembly Code
- Computers execute *Machine Code* which is difficult for humans to read, write and debug as it is in Binary
	- An instruction in Machine Code may look like: 01000101
- **Assembly Code** instructions are equivalent to machine code but easier for humans to work with
	- An instruction in Assembly Code may look like: LDA 5

## Assembler
- Assembly Code is a *low level language*
- Translating assembly code instructions into machine code is done by an **assembler**
- Each processor has its own instruction set and so the *object code* produced will be hardware specific ![[Pasted image 20250314093509.png]]
## Compiler
- A **compiler** translates a whole program written in a *high level language* into executable *machine code*, going through several stages
	- Compiled high level languages include C++, C, Rust
- The resulting machine code is called *object code*
- The object code produced is *also* hardware specific ![[Pasted image 20250314094003.png]]
## Interpreter
- An **interpreter** also translates code written in a *high level language* into *machine code*
	- Interpreted high level languages include Python, JavaScript and PHP
- **However**, the **interpreter** does this *line by line* rather than translating the whole program before any of it can be executed ![[Pasted image 20250314100315.png]]
## Compiler Vs Interpreter

| Compiler                                                    | Interpreter                                                        |
| ----------------------------------------------------------- | ------------------------------------------------------------------ |
| Program can be run many times without the need to recompile | Source code can be run on any machine with the interpreter         |
| Faster to execute                                           | If a small error is found, no need to recompile the entire program |
| Executable code does not require the interpreter to run     |                                                                    |
| Compiled code cannot be easily read and copied by others    |                                                                    |

# Bytecode
- Most languages are not solely *compiled* or *interpreted*; they use a combination of *both*
- For example, Java is compiled into **bytecode** which is an *intermediate* step between **Source Code** and **Machine Code**
- The **bytecode** is interpreted by a bytecode interpreter, for example the Java Virtual Machine (JVM)![[Pasted image 20250314094740.png]]

# Stages of Compilation
- There are several steps that a **compiler** goes through to convert source code to object code
## Lexical Analysis
- All unnecessary spaces and all comments are removed
- Keywords (print, for example), constants and identifiers are replaced with **tokens** representing their function in the program
- For example, this code:
	- `age = 17; print (age)`
	- This would produce the following tokens:
	- `<identifier> <operator> <number> <keyword> <open_bracket> <identifier> <close_bracket>`
## Symbol Table
- The **lexer** will build a symbol table for every keyword and identifier in the program
- The symbol table helps to keep track of the run-time memory address for each identifier ![[Pasted image 20250314101501.png]]
## Syntax Analysis
- The stream of tokens from the *lexing* stage is split up into **phrases**
- Each phrase is **parsed** which means it is checked against the rules of the language
- If the phrase is not valid, an error will be recorded
	- For example, this sequence of tokens may not be valid and this would be picked up by **syntax analysis**
	- `<number> <operator> <identifier>`
	- The source code might be `5 = a`
## Syntax Rules
- The rules of the language need to be defined
- **Syntax rules** can be drawn as a syntax diagram ![[Pasted image 20250314101828.png]]

## Semantic Analysis
- It is possible to create a sequence of *tokens* which is *valid* syntax but *not* a *valid* program
- **Semantic Analysis** is responsible for checking this kind of error
	- For example, this phrase may be valid syntax;
	- `<if> <identifier> <operator> <number>`
		- the source code might be: `if a > 5`
	- *However*, if the identifier has not been previously declared, then semantically, it is not a valid program
## Code Generation
- Once the program has been checked, the compiler generates the machine code
- It may do this in several 'passes' over the code because **code optimisation** will also take place
## Code Optimisation
- There are times when the *source code* is written inefficiently
- **Code optimisation** aims to:
	- Remove *redundant* instructions
	- Replace *inefficient* code with code that achieves the *same result* in a *more efficient* way

# Libraries
- Most languages have sets of pre-written (*and pre-compiled*) functions called **libraries**
- Examples could include functions for generating random numbers or for mathematical operations
- A programmer can also write their own **libraries**
- **Library** functions can be called within a program
# Linker
- The **linker** needs to put the appropriate memory addresses in place so that the program can call and return from a library function ![[Pasted image 20250314110016.png]]
# Loader
- The job of the **loader** is to copy the program and any linked subroutines into main memory to run
- When the executable code was created, it may assume the program will load in *memory address 0*
- However, memory addresses in the program will need to be *relocated* by the **loader** because some memory will already be in use
# Related Notes
[[Computer Science MOC]]
[[CS - NY - Systems Software and Applications Generation]]