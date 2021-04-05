# Conditional Assignment Statements
Models for higher abstraction are difficult to express with Concurrent Signal Assignment statements, VDHL provides Conditional Assignment Statements for these situations.

- Evaluation takes place in the order that they appear.
- The first true condition determines the output.
- The order should reflect the physical implementation.

# Selected Signal Assignment
Similar to case statement in conventional languages.

- Choices are not evaluated in sequence.
- Only one must be true.
- The statement must cover all possible combinations.
- The ``others`` clause must be used in situations where not all possible combinations are covered by the select statements.
- ``unaffected`` may also be used in this type of statement.
