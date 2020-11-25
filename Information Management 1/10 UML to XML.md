# UML to XML

## XML MetaData Interchange: XMI
Standard sponsored by the OMG. Originally for allowing interchange of UML models between UML editors. Now seen as a sensible XML representation of UML for other purposes.

## UML Class Mapping
Each instance of a UML class produces one XML element. UML class name translates to XML tag name.

Be careful in naming your UML classes as XML has restrictions on valid tag names:
- Cannot contain spaces
- Alpha or Number characters but also full stop, dash or underscore
- Can begin with letter or _
- CANNOT begin with letters "XML" !!

## UML Attribute Mapping
Each attribute of a UML class produces a child XML element.

Element name is made unique by prepending with the class name.

XML has no representation for multivalues attributes of UML so these attributes are translated into individual XML elements.

## UML Inheritance Mapping
Current XML standards do not have built in mechanisms for representation of inheritance

The XMI Standard specifies use of copy down approach for generalisations, attributes, association refs and compositions. The is definitions from all superclasses are copied down to the class being translated into XML.

## UML Associations
A reference to the class of the associated class is included in the definition using the `xmi.idref` attribute.
