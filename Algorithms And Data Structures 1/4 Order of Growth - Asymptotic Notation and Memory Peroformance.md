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
