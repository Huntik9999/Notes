---
title: What is OpenGL?
tags:
  - "#OpenGL"
  - First_Chapter
updated: 2025-08-09
---
# What Is OpenGL?

- OpenGL is not an API but a specification  
	- **Specification** - what something does
	- managed by Khronos Group
- Developers come up with Implantations
	- **Implementation** - how something does the specification
	- Maintained by graphics card companies(Nvidia, Apple, Intel) 

---

## Core-profile vs Immediate Mode

- Immediate Mode - easy - less control
- Core-profile - hard - flexible & efficient
- Newer versions of OpenGL create more efficient systems for task
- Newer version = Newer graphics card requirement 

---

## Extensions 

- graphics companies create new technique or large optimizations implemented in drivers
	- can be enabled for advanced or efficient graphics
- based on support for a hardware 
	- use if else statement to check if available 
- popular extensions become part of OpenGL

---

## State Machine 

- OpenGL is a state machine
	- collection of variables that define how OpenGL should currently operate 
- State of OpenGL = OpenGL context
- We can tell OpenGL to draw lines instead of triangles 
- Comes with state-changing functions for changing the context

---

## Objects

- OpenGL library is written in C 
- Object is a collection of options
	-  can be visualized as structs
	- represents subset of OpenGL's state 
- create object -> store reference as a id -> bind object to target location of context 
- can define more than one object 