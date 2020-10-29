# Strings

Strings are simply arrays of characters.

By convention, C uses a NULL character `'\0'` to terminate all strings in its library functions.

It's the string terminator (not the size of the array) that determines the length of the string.

It's possible to have String literals as a string quoted by double brackets. This can be used to initialise a character array.

## Printing with printf()
`printf` expects to receive a string as an additional parameter when it sees `%s` in the format string.

`printf` knows how much to print out because of the NULL character at the end of all strings.

## Printing with puts()
The `puts` functions is a much simpler output function than `printf` for string printing.

## Inputting Strings with fgets()
`fgets()` gets a line from a file.

## The C String Library
Sting functions are provided in an ANSI standard string library.

```c
 #include <string.h>
```

Includes functions such as:
- Computing the length of a string
- Copying strings
- Concatenating strings

The library is guaranteed to be there in any ANSI standard implementation of C.

### strlen
`strlen` returns the length of a NULL terminated character string.

```c
size_t strlen(char * str);
```

`size_t` is a type defined in string.h that is equivalent to an unsigned int.

### strcpy
```c
char *strcpy(char * destination, char * source);
```

A copy of `source` is made at `destination`. The return value also points at the `destination`.
