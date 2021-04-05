# Pointers Continued Continued

## Allocating Memory at Execution Time
- When we declare local variables, the memory for those variables is allocated automatically.
  - Each of these variables has a name.
  - We can get the address of local variables using the `&` operator.
  - We can refer to a variable using either its name or the pointer to it.
- We can create variables that have no name, called **anonymous variables**.
  - We refer to these variables *only* with pointers.
  - An anonymous variable without a pointer is unreachable.
  - You never declare anonymous variables.
  - Allocated using `malloc()`.

## Dynamically-Allocated Arrays
In the original C standard arrays had to be of a constant size, but since C99 standard, the size can be a variable expression.

However you can use `malloc()` to allocate a block of memory of any size.
- The result of `malloc()` is always stored in a pointer.
- In C pointers can be treated very much like arrays.

Dynamically created arrays can be used and passed around just like regular arrays, the main difference is that the dynamically created arrays are anonymous variables. Therefore, when you are finished with a dynamically created array, you must release it explicitly.
