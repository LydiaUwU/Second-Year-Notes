# Document Type Definition (DTD)

- Defines structure/model of XML documents:
 - Elements and Cardinality
 - Attributes
 - Aggregation
- Defines default attribute values
- Defines Entities
- Stored in a plain text file and referenced by an XML document (*external*).
- Alternatively a DTD can be placed in the XML document itself (*internal*).

## Define Type Declaration
Define occurrences of elements:
- `?`: zero-or-none
- `+`: one-or-more
- `*`: zero-or-more

## XML Namespaces & XML Schema
DTDs use a non-XML syntax and have a number of limitations:
- No namespace support
- lack of data-types

XML stemas are an alternative to DTDs that support simple and complex data-types

## Why use XML Schemas?
- Uses an XML syntax.
- Supports simple and complex data-types such as user-defined types.
- An XML document and its contents can be validated against Schema.
- Can validate documents containing multiple namespaces.
- Schemas are more powerful than DTDs and will eventually replace DTDs.
