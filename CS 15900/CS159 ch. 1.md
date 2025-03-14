---
tags:
  - videonotes
  - S2
  - cs159
Type: Video Notes
Date: 2025-01-21
Class: "[[CS 15900]]"
---
- computer made of cpu, main memory, i/o, systems interconnection
	- cpu: processes the instructions that we program
		- registers: memory close to the processor, allowing it to store data and instructions near to it so as to be accessed easily
		- arithmetic/logical unit: handles the math (data manipulation) the program is executing
		- control unit
		- internal interconnections
			- cpu coordinates and performs operations of the computer
			- instructions of operations are interpreted and executed in the **instruction cycle**
![[Pasted image 20250121215158.png|400]]

- memory ("secondary memory"): instructions and data
	- memory hierarchy
		- data and instructions must make their way thru different levels of memory. the higher the level, the higher the performance but the lower the capacity
		- secondary memory -> primary memory, main memory, ram -> cpu registers
---
- natural languages: what we use to talk to each other
- machine languages: that which the computer understands
	- high/low level programming languages 
- programming languages lie in between natural/machine languages 
	- use familiar terms from natural languages as important part of instructions
	- degree of high/low depends on how a programming language is (1) close to the natural language and (2) how far removed from any specific hardware.
	- "higher" degree uses more "natural" languages, code specifically to the hardware
- process of writing a program composed of following steps
	1. write or edit source code
	2. save changes
	3. compile source code (turns into machine language to generate an executable)
	4. test/run the executable file 
- compiling fails when you violate the rules of the syntax
	- preprocessor prepares the program for the remainder of the compiling process
		- commands (directives) can be given to the preprocessor
- each time you compile successfully a new executable file, also named a.out, will replace any existing a.out file in the same directory
----
planning out the design of a code is very important
1. what are I/O requirements?
2. analyze the problem
3. design the algorithm: use flowcharts to visually represent them (structure chart used for decomposition (..?))
	- terminal symbol: rounded rectangle serves as start/end of algorithm
	- assignments: mathematical expressions, calculations. rectangle
	- I/O: parallelogram serves to designate data for input/output
	- conditional expressions: diamond used to show T/F. make sure to label T/F paths 
	- connector: oval used to show repetitions 