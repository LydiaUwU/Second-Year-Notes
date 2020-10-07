# Arrays

## Single Dimensional Arrays
```c
typename variablename[size];
```

## Using Constants to Define Arrays
It is useful to define arrays using *constants*.

In GNU C, the variable length array is allowed.
In ANSI C, the handling of variable length arrays is more complicated.

## Array-Bounds Checking
C, unlike many languages, does **NOT** check array bound subscripts during compilation and runtime.

If you access off the ends of any array it will calculate the address it expects the data to be at, and then attempts to use it anyways.

It is the programmer's responsibility to ensure that their programs are correctly written and debugged.

## Initialising Arrays
```c
int array[4] = {1, 2, 3, 4};
```

## Multidimensional Arrays
```c
int array[2][3] = {{1, 2, 3}, {4, 5, 6}};
```

## The Value of the Array Name
When the array name is used alone, its value is the address of the array, `&array` is the address at which the pointer to the array is stored.
