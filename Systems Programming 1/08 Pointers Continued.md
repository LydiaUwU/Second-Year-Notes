# Pointers Continued

## Pointer Arithmetic
When a pointer variable points to an array element, there is a notion of adding or subtracting an integer to/from the pointer.

You can add and subtract pointers, but you can't directly multiple or divide them. *(check if you can mod them)*

If two pointers point to elements of the same array, then there are notions of subtraction and comparisons between two pointers.

## Pointers and Arrays
Recall that the value of an array name is also an address. In fact pointers and array names can be used interchangeably in many cases.

An array name is like a constant pointer, which points to the first element of the array. Therefor you can "pass an array" to a function.

### Two major differences
- Array names come with valid spaces where they "point" to and you cannot 'point' the names to other places.
- Pointers do not point to valid space when they are created. You have to point them to some valid space (initialisation).
