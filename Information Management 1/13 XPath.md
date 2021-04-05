# XPath

XPath is used for navigating XML documents.

> XPath, essentially specification of path for walking the XML tree

Simple path expression is a sequence of steps to walk the tree. The sequence of steps are separated by slashes.

If an XPath expression begins with `//` it selects nodes in the document from the current node that match the selection no matter where they are.

## String Function
Using the `string()` function to get just the text from any relevant elements.

## Attribute @
Attributes are referred to by putting an `@` symbol before the name, and appear in the path as if nested within the tag.

## Predicate Filters []
A part of the path that allows for expression of a condition. `[...]` will ensure that only nodes that satisfy the condition are included in the resultant set.

## Wildcard *
A `*` can be used as a wildcard.

## Selecting Several Paths |
By using the `|` operator in an XPath expression you can select several paths.
