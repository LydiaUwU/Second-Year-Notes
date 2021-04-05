# Parts of an XML Document

## Elements
Define logical structure and sections of XML documents,

Difference content types:
- Attribute content
- Text content
- Element content
- Empty

Each element must be completely enclosed by another element, except for the root.

Any element name must start with a letter or underscore but after that can include also digits, fullstops, hyphens.

Dont start with colon due to namespaces.

Dont include spaces.

## Attributes
Provides additional information about an element.

Attributes are contained within the *start-tag*.

Consists of a name and associated value separated by an equals sign.

The attribute value must always be enclosed by quotes.

The order of attributes is insignificant.

## Entities
Storage units for repeated text.

*Built-in Entities* are also used for special characters that cannot be typed directly in an XML document.

## Character Data Sections
Data which is to be parsed is called PCDATA.

An XML parser will not treat the contents of a CDATA section as markup.

Entity references are not resolved in CDATA sections.

Useful for including source code in XML.

## Comments
Used to comment XML documents.

Not considered to be part of an XML document.

An XML parser is not required to pass comments to higher level applications.

## XML Declaration
Placed at the start of an XML document.

Informs XML software of:
- The version of XML the document conforms to.
- The character encoding scheme used in the document. 
- Whether or not a set of external declarations affect the interpretation of this document.
- Whether external declarations are public or private.

## Well Formed XML
- XML Declaration required.
- At least one element.
  - Exactly one root element.
- Empty elements are written in one of two ways:
  - Closing tag `<Name></Name>`
  - Special start tag `<Name/>`
- For non-empty elements, closing tags are required.
- Attribute values must always be quoted.
- Start tag must match closing tag.
- Correct nesting of elements.
