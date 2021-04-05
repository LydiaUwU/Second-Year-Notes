# Expression and Operators

An expression in C usually has a value unless it is a function call that returns `void`.

### Two Types
- Function Calls.
- The expressions formed by data and operators.

## Arithmetic Operators
- `+` Addition
- `-` Subtraction
- `-` Negation
- `*` Multiplication
- `/` Division
- `%` Modulus

## Assignment Operator
`=` is an operator.

## Compound Assignment Operator
We can combine arithmetic and assignment operators to create compound assignment operators.

## Increment and Decrement
`++` and `--`. Changes a value by 1.

## Side Effects
In C it is easy to write an expression with multiple side effects. Using expressions with side effects was once idiomatic C but we now know better.

*You should not use expressions with multiple side effects.*

### Implementation Defined
C implementation must choose some behaviour, this behaviour must be documented.

### Unspecified Behaviour
C implementation must choose some behaviour, which does not need to be documented.

## Rational Operators
Operators for comparing variables.

- `==` Equals
- `>` Greater Than
- `<` Less Than
- `>=` Greater Than or Equal To
- `<=` Less Than or Equal To
- `!=` Not Equals

## Logical Operators
- `&&` AND
- `||` OR
- `!` NOT

## Operating on Bits
- `<<` Shift Left
- `>>` Shift Right
- `&` Bitwise AND
- `|` Bitwise Inclusive OR
- `^` Bitwise Exclusive OR
- `~` The Complement Operator

C allows you to operate on the bit representation of integer variables.

In C, hexadecimal literals begin with `0x`, and octal literals begin with `0`.

*Beware of bitwise operators and signed numbers*

## Shift, Multiplication and Division
**Dont try this at home!**

Multiplication and division are often slower than shift, and multiplication or division by 2 can be replaced by shifting 1 bit to the left/right.

*An optimising compiler will make this transformation automatically!*

## Conditional Operator
Same as the java conditional operator.

`exp1 ? exp 2 : exp3`

## Comma Operator
An expression can be composed of multiple subexpressions separated by commas.

The comma operator is often used in `for` loops
