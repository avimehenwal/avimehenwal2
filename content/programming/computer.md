---
title: How does a computer work
tags:
  - computer
  - electronics
---

# How does a Computer Work?

<TagLinks />

Creating a design of a house can be considered as **computer architecture**,
whereas building the house can be considered as **computer organization.**

- Charge, current
- Diod
  - How do junctions work?
  - Doping process?
  - Forward and Backward biased
- Transistor, BJT, MOSFET, CMOS
- Logic Gates
- Flip Flops - Registers
  - How to we save config in system. Design memory
- S-RAM, D-RAM
- Boolean Algebra - CPU Logic
  - Control Unit
  - Arithmetic And Logic Unit
- ISA - Instruction Set Architecture
  - operations and microoperations
    - load, store, jump, **aluops**
  - [ISA Comparision](https://en.wikipedia.org/wiki/Comparison_of_instruction_set_architectures)
- CPU Architectures
  - Flynn Taxonomy SISD, SIMD, MISD, MIMD
  - vector architecture
- How do we tell CPU what to do?
  - Programming
  - levels of Programming
- How does CPU keep track of multiple instructions
  - CPU Clock synchronization
  - CPU Pipelining
  - Tomosulos algorithm
- Memory Hierarchy

::: quote
At the end of the day, linux wants to make software and windows wants to make money
:::

> Software make for society

- Computer only understand 0 and 1, unreadable for humans
  - Assembly level languages - ==Opcode mnemonics==
    - more redable than machine code
  - `ADD R1 R2`
  - use hexademical, decimal and octal number system for representing 0's and 1's
- Assemly is hard to write by humans, keeping track of all memory locations and pointers
- Enter Compilers
  - [First Compiler?](https://stackoverflow.com/questions/1653649/how-was-the-first-compiler-written)
  - [Grace Hopper A-0 compiler](http://www.computinghistory.org.uk/det/5487/Grace%20Hopper%20completes%20the%20A-0%20Compiler)
- How to process the opcodes? Hardware problem
- How we generate opcoddes? - COmpiler Backend problem
- GNU Compiler COllection GCC, LLVM
  - [history of compiler](https://en.wikipedia.org/wiki/History_of_compiler_construction#:~:text=The%20first%20practical%20compiler%20was,modern%20notion%20of%20a%20compiler.)
- Then came more hardware peripherals
- Operating System
  - Drivers
  - Firmware
  - Application Software
- Why did we have to put `;` at the end of each line?
  - to make it easy for parser to break instructions

::: tip Whats the difference?
Machine Code | Bytecode | Assembly Code?
:::

Machine code is generally different from bytecode (also known as **p-code**), which is either executed by an interpreter or itself compiled into machine code for faster (direct) execution. An exception is when a processor is designed to use a particular bytecode directly as its machine code, such as is the case with Java processors.

Machine code and assembly code are sometimes called **native code** when referring to platform-dependent parts of language features or libraries

## questions

- How to count the #lines of machine code written by a program?
  - for source code [cloc](https://github.com/AlDanial/cloc)
- How to print the machine code?

```c
gcc -o fib fib.c
otool -tv fib
```

## Why do people contribute to opensource?

1. I want to solve a problem
2. I want to build my reputation
3. I feel like I belong here, found their tribe
4. Its fun for me
5. I am learning

## Rust vs C++

- **90,000 bugs** in C++ source code
- All gaming engines are in `C++`

## Resources

- [Assembly Programming primer](https://www.nayuki.io/page/a-fundamental-introduction-to-x86-assembly-programming)
- [IA-32 ISA Datasheet](https://www.intel.com/content/dam/www/public/us/en/documents/manuals/64-ia-32-architectures-software-developer-instruction-set-reference-manual-325383.pdf)

<iframe width="560" height="315" src="https://www.youtube.com/embed/d9SWNLZvA8g" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<Footer />
