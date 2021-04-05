# XQuery

XQuery is for querying XML documents.

Originally focused on retrieval of information from XML documents.
- Update features added in 2011.

XQuery is a language for finding and extracting elements and attributes from XML documents, used in conjunction with XPath.

## For-Let-Where-OrderBy-Return "FLWOR"

1. One or more FOR and/or LET expressions for gathering nodes into a set from a series of XPath queries to operate upon other clauses.
2. Optional WHERE clause for filtering nodes in the sets to be operated upon in other clauses.
3. Optional ORDER BY clause for returning nodes in the sets in particular order in other clauses.
4. RETURN clause for returning the identified nodes in the sets.

## FOR Clause
```
FOR <variable> IN <xpath expression>, <xpath expression>, ...
```

Variable (starting with `$`) "binds to" in turn each member in the set returned by XPath expression(s).
For each variable binding the rest of FLOWR expression is executed.
More than one variable/path expression binding can be specified by separating with comma.

## LET Clause
```
LET <variable> := <xpath expression>, <xpath expression>, ...
```

Variable (starting with `$`) "binds to" the set returned by XPath expression.
Does not iterate over the set like FOR clause does.
It cannot be redefined within the scope of the function.
More than one variable/path expression binding can be specified by separating with comma.

### RETURN Clause
One limitation of XPath is that it can only operate on existing elements/attributes within the document.

XQuery allows the generation of new elements/attributes nodes.
- The element's content is either literally given between start- and end-tag, or provided as an "enclosed expression", or as a mixture of both.
- Curly brackets are used for enclosed expressions in the return clause and indicate that the expression enclosed needs to be evaluated by the XQuery processor.

## WHERE Clause
Filters the binding tuples produced by the FOR and LET clauses. If the filter expression evaluates to true then the RETURN clause is executed.

## XQuery Sorting
The return clause of a FLWOR expression is evaluated once for each tuple in the tuple stream, and the results of these evaluations are concatenated to form the result of FLWOR expression.
- If no order by clause is present, the order of the tuple stream is determined by the orderings of the sequences returned by the expressions in the for clauses.
- If an order by clause is present, it determines the order of the tuple stream.

## Sequence Operations
**Union:** Of two node sequences is a sequence containing all the nodes that occur in either of the operands.

**Intersect:** Operator produces a sequence containing all the nodes that occur in both of its operands.

**Except:** Operator produces a sequence containing all the nodes that occur in its first operand but not its second operand.

## Conditional Clauses
```
if (test expression) then expression else expression
```

The result of a conditional expression depends on the value of the test expression in the if clause.
- If the value of the test expression is the Boolean value true, or a sequence containing at least one node (serving as an "existence test") then the clause is executed.
- If the value opf the test expression is the Boolean value false or an empty sequence, the else clause is executed.
**All three clauses (if, then, and else) are required**

## Quantified Expression
Allows a variable to iterate over the items in a sequence. For each variable binding a test expression is evaluated.
- A quantified expression that begins with `some` keyword returns the value true if the test expression is true for some variable binding.
- A quantified expression that begins with `every` keyword, returns the value true if the test expression is true for every variable binding.

## User Functions
XQuery allows users to define functions of their own.
- A function may take zero or more parameters.
- A function definition must specify the name of the function and the names of its parameters if they exist.
  - It may optionally specify types for the parameters, if no type is specified for a function parameter, that parameter accepts values of any type.
  - It may optionally specify types for the result of the function, if not type is specified for the result of the function, the function may return a value of any type.
- Body of the function is an expression enclosed in curly braces with a semicolon following the closing bracket.

## Types in Queries
Sometimes its necessary to refer to a particular type in a query.
One way to refer to a type is by its qualified name, or QName.
- A QName may refer to a built-in type such as `xs:integer` or to a type that is defined in some schema, such as `abc:student`.
- If the QName has a namespace prefix (the part to the left of the colon), that prefix must be bound to a specific namespace URI using the "declare namespace" clause.

Another way to refer to a type is by a generic keyword such as element or attribute.
- May optionally be followed by a QName that further restricts the name or type of the node.
- A reference to a type may be optionally followed by one of three occurrence indicators.
