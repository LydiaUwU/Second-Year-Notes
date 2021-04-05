# Flow Control

## Comments
**Syntax:** `/* This is a comment */` & `// so is this`

- Comments should explain:
  - Special cases.
  - The use of functions (parameters, return values, purpose).
  - Special tricks or things that are not obvious.
- Explain *what* your code does.
- Explain *why* your code does the things that it does.

## Compound Statements
Sequences of statements that can be combined into one with `{...}`.

## C Statements
- **DO:** Stay consistent with whitespace.
- **DO:** line up block braces so that it is easy to find the begininning and end of a block.
- **DO:** Use blank lines to separate code into logical blocks.
- **AVOID:** Spreading a single statement across multiple lines if there is no need.
- **DO NOT:** Put blank lines between every statement.

## If Statements
Pretty much identical to Java.

## For Statements
Pretty much identical to Java.

## While Statements
Pretty much identical to Java.

## Do-While Statements
Pretty much identical to Java.

## Which Loop Should I Use?
- Different loops mean different things to the reader.
- Use for loops to visit all of a range of values.
- Use while loops for more complicated loops.
- Use do-while loops if the loop is always done once, and this is difficult to express with a while loop.

**Do Not:** Modify the loop control variable within a for loop.

## Break
The flow of control in any loop can be changed through the use of the `break` and `continue` commands.
The `break` command exists the loop immediately. Useful for stopping on conditions not controlled by the loop condition.

Occasionally used to break out of infinite while loops.

## Continue
The `continue` statement causes the next iteration of the loop to be started immediately.

## Switch Statements
Pretty much identical to Java.

## Goto Statements
The `goto` statement will jump to any point in the same function.

**Do Not:** Jump into a loop!
**Do Not:** Jump backward!

- The `goto` statement is very powerful, you can jump anywhere within the current function.
- Using a `goto` is never necessary.
- A lot of `goto` statements make spaghetti code.
- Expect other people to rewrite code to remove the `goto`.
- Expect to take massive abuse from other programmers.
