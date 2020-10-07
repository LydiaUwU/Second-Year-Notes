# Order-of-Growth

## Common Order-of-Growth Classifications
**Definition:**  If ``f(N) ~ c g(N)`` for some constant ``c > 0``, then the order of growth of ``f(N)`` is ``g(N)``.

**Good News:** The set of functions:

``1,  log N,  N,  N log N,  N^2,  N^3, and 2^N``

suffices to describe the order of growth of most common algorithms.

**Linear:** Each iteration of a loop reduces the boundaries of a loop by a constant.

## Example: Binary Search
**Binary Search:** Compare key against middle entry.
- Too small, go left.
- Too big, go right.
- Equal, found.

## Logarithms
- The base of the logarithm contributes only a constant factor to the running time, it does not contribute to the Order-of-Growth.

# Asymptotic Notation
In the Theory of Algorithms we are interested in the order of growth of runtime `T(N)`, expressed as a function of input size `N`.

`T(N)` may not be a simple function and can have different orders of growth for different values of `N`.

### Rationale for Asymptotic Notation
- Larger `N`s are more important than smaller ones.
- Consider the order of growth when `N` approaches infinity.

## Types of Notation
**Big Theta:** The set of functions with asymptotic order of growth `g(N)`.
**Big O:** The set of functions with asymptotic order of growth less than or equal to `g(N)`.
**Big Omega:** The set of functions with asymptotic order of growth greater than or equal to `g(N)`.

## Common Mistakes
1. Interpreting O/Theta/Omega as worst/average/best case running times.
2. Interpret asymptotic notation as an approximate model. *Tilde notation is an approximate model*
