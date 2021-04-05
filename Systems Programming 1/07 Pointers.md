# Pointers
When a variable is defined the compiler (linker/loader actually) allocates a real memory address for the variable.

When a value is assigned to a variable, the value is actually placed to the memory that was allocated.

When a value of a variable is used, the contents in the memory are used.

The address can be passed to a function and can also be stored in a variable.

## Declaring Pointers
```c
type * pointername;
```

For example:

```c
int * p1;
```

## Initialising Pointers
*Like other variables, always initialise pointers before using them!*

## Using Pointers
You can use pointers to access the values of the other variables.

## Pointers as Function Parameters
Sometimes you want a function to assign a value to a variable. You can use global variables but this makes the function non-reusable. Instead you can pass pointers into functions as parameters.
