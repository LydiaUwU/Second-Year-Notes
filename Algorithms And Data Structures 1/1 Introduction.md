# Introduction to algorithms and Data Structures 1

Objective: Learn to solve computational problems efficiently

> Algorithms + Data Structures = Programs

**Algorithm**: The steps to correctly perform a task that answers a general computation problem
**General**: The algorithm should work regardless of the specific input
**Data Structures**: The ways to store the information needed for the algorithm.
*E.g. Arrays, Linked lists, Hash Tables, Binary Trees, etc.*

## Programs
- Must be correct.
  - Mathematical guarantee of correctness only through Formal Verification.
  - Confidence of correctness through testing.
    - In CSU22011 (and in the SW industry): **Unit Testing**.
    - Other kinds of testing: *integration testing, validation testing, user testing, etc.*
- Must be efficient.

## Efficiency
### Measures of Efficiency.
**Established Measure**: How well the program scales to larger inputs.
- When I *double* the input size my program takes *the same* time to run on the same computer (*Constant Running Time*).
- When I *double* the inout size my program takes *twice* the time to run on the same computer (*Linear Running Time*).

We also care about the memory needed:
- When I *double* the input size my program needs *the same* amount of memory to run (*Constant Memory Space*).
- When I *double* the input size my program takes *twice* the amount of memory to run (*Linear Memory Space*).

Scalability may some times seem crude but allows us to at least compare algorithms.

## Overview
- Learn about the most common A&DS that every CS graduate must know.
  - *E.G Merger Sort, Union-Find, Dijstra's Shortest Path Tree, etc.*
- Identify which known A&DS structures best fit specific problems.
- Learn Abstract Data Types: interfaces of A&DS.
- Practice implementing A&DS through labs and practical assignments.
- Learn to evaluate new algorithms.
  - Efficiency: calculate the running time and memory usage.
    - How well they scale.
    - Measuring Aspects: *Worst-case, average-case, amortised, experimental performance.*
    - Measuring Systems: Big-O notation.
  - Correctness.

We will be using Java in this course.

## Course Logistic
Primary Website: <https://mymodule.tcd.ie>

08:00-09:00 is a placeholder for pre-recorded lectures.
Labs will be for asking questions about the assignments.
Assignments will be graded using Web-CAT and multiple submissions are accepted.

## Example Problem
A software engineer was asked to design an algorithm which will input two **unsorted** arrays of integers, **A** (of size *N*) and **B** (also of size *N*), and will output `true` when all integers in **A** are present in **B**.

The engineer came up with **two** alternatives. (*In slides*)
