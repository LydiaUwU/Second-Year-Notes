# Analysis of Algorithms

We will likely not be talking about average assumptions in this class.
In this module (and usually in programming practice) we will focus on the **worst-case inputs**.

## Why Analyse Algorithms
**Good Programmer:** To predict the performance of our programs.
**Good Client:** To choose between alternative algorithms/implementations.
**Good Manager:** To provide guarantees to clients.
**Good Scientist:** To understand the nature of computing.

## Evaluating Running Times
1. **Scientific Method:** Measure running times through experiments.
2. **Mathematical Methods:** Consider a convenient model of computation and:
  - Sum up the number of program steps for **worst-case** inputs of size `N`.
  - Calculate the number of program steps for **worst-case** (FILL THIS IN)

## Running Time
### Some Algorithmic Successes
#### Discrete Fourier Transform
- Break down waveform of N samples into periodic components.
- Applications: *DVD, JPEG, MRI, astrophysics, ...*
- Brute Force: `N^2` steps (*quadratic*).
- FFT algorithm: `NlogN` steps (*linearithmic*).

#### N-Body Simulation
- Brute Force: `N^2` steps.
- Barnes-Hut Algorithm: `NlogN` steps.

## The Challenge
*Q.* Will my program be able to solve a large practical input?

## Scientific Method Applied to Analysis of Algorithms
A framework for predicting performance and comparing algorithms.

### Evaluating Algorithms Through Experiments.
We can measure the running time using Java's `Stopwatch` and its method `elapsedTime()`.

### Data Analysis
**Standard Plot:** Plot running time `T(N)` vs input size `N`.
**Log-log Plot:** Plot running time `T(N)` vs `N` using **log-log scale**.
  - **Regression:** For straight line through data points: `aN^b`

### Doubling Hypothesis
**Doubling Hypothesis:** Quick way to estimate `b` in a power-law relationship.

## Experimental Algorithmics
### System Independent Effects.
- Algorithm
- Input Data

Determines exponent in power law.

### System Dependent Effects.
- Hardware: *CPU, Memory, Cache, ...*
- Software: *Compiler, Interpreter, Garbage Collector, ...*
- System: *Operating System, Network, Other Apps, ...*

**Bad News:** Difficult to get precise measurments.
**Good News:** Much easier and cheaper than other sciences. *E.g. Can run a huge number of experiments.*
