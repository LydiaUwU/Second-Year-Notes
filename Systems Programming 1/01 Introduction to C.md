# Introduction to C

## A Brief History
Created by Dennis Ritchie at AT&T labs in 1972.
Designed as a portable replacement to assembly.
C is a small simple programming language, originally only had 27 keywords
Easy to write a simple compiler for C, and is a standardised language.

## Why learn C?
- C operates on memory at the machine level.
  - Programming in C gives you a good understanding of how data is organised in memory.
- C is a widely-used language.
- C is a lingua franca (*communication language*).
  - It's easy to communicate your ideas to others in C.
  - There is a C compiler for almost every processor.
  - Many other languages are implemented by compiling to C.
- C gives you much of the control of assembly.
  - You can achieve nearly the efficiency of assembly code.
  - System calls and pointers allow you to do most of the things that you can do with an assembly language.

## 'Hello World'
```
#include <stdio.h>
// print a message
int main() {
        printf("Hello cruel world!\n");
        return 0;
}
```

## Compilation
To compile a program:
- Compile the program to object code.

``clang -c hello.c``

- Link the object code to executable file.

``clang hello.o -o hello``

You can do the two steps together by running:

``clang hello.c -o hello``

To run your program:

``./hello``
