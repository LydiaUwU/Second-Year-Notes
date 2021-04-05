# Basic Types and Formatted IO

## C Variable Names
- Variable names may contain letters, digits and underscores.
- The first character must be a letter or an underscore.
  - The underscore can be used but **watch out!**
- Case sensitive.
- C keywords may not be uses as variable names

Suggestions regarding variable names:
- **DO:** use variable names that are descriptive.
- **DO:** Adopt and stick to a standard naming convention.
- **DO:** Use short names for local variables.
- **DO:** Use long names for global variables.
- **DO:** Use standard names for common idioms. *E.g. i, j, s, t, result, etc.*
- **AVOID:** Variable names starting with an underscore, often used by the operating system.
- **AVOID:** Using uppoercase only variable names, generally these are pre-processor macros.

## C Basic Types
![C Basic Types Table (*In notes*)](/Images/C-Basic-Types.png)

## Formatted Printing with printf
The `printf` function is used to output information (both data from variables and text) to the standard output

`printf(format string, arg1, arg2, ...);`

The format string contains:
- **Literal Text:** is printed as is without variation.
- **Escaped Sequences:** Special characters preceded by `\`.
- **Conversion Specifiers:** `%` followed by a single character.
  - Indicates that a variable is to be printed at this location in the output stream.
  - The variables to be printed must appear in the parameters to `printf` following the format string, in the order that they appear in the format string.

## Reading Numeric Data with scanf
- The `scanf` function is the input equivalent of `printf`.
  - A C library function in the <stdio.h> library.
  - Takes a format string and parameters, much like `printf`.
  - The format string specifiers are *nearly* the same as those useing in `printf`.
    - **Important Exception:** Double values are specified with `%lf`.
- The ampersand is used to get the adress of the variable.
  - All of the C function paramters are "passed by value."

Bizarrely, `%ld` must be used with `printf` but `%lf` must not.

## Type Conversion
C allows for conversions between the basic types implicitly or explicitly.
Explicit conversion uses the cast operator.

## Implicit Conversion
If the compiler expects one type at a position, but another types is provided, then implicit conversion occurs.

**Arithmetic Conversion:** If two operands of a binary operator are not the same type implicit conversion occurs.

## The sizeof() Function
The `sizeof()` function returns the number of bytes in a data type.

## Creating Simple Types
`typedef` creates a new name for an existing type.
  - Allows you to create a new name for a complex old name.

### Generic Syntax
``typedef oldtype newtype``

These are often used with complex data types and can simplify syntax.

## Variable Declaration
### Generic Form
``typename varname1, varname2, ...;``

Declaration outside of any function are for global variables.

**Always** initialise a variable before using it!

**Warning:** be careful about "out of range errors".

## Constants
You can also declare variables as being constants using `const`.

Some people say that the only literal value in your code without being a named constant is `0`.

## Preprocessor Constants
These are an older form of constant.

### Generic Form:
``#define CONSTNAME literal``

## Literals in C
Literals are representations of values of some types.
