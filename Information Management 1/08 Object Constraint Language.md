# Object Constraint Language and Varying UML Notation
UML is Technology Neutral.

## Constraints
- Constraints on UML Model Elements
  - Conditions/Criteria that must be true about some aspect of the system.
- Constraints will make the analysis and design more precise and rigorous
- Complement the UML graphical notation and can be useful to use with *all* model elements.
- Helps with verification and validation of models.
- Helps with communication of intent of some aspect of the model.

Each OCL constraint has a context, the element that is being constrained.

A constraint can be written in a textual form or attached to model elements as a note.

Keyword `context` in a bold type.

The keyword `self` in the textual form of the constraint simply refers to the insance of the context class.

**Invariant:** Constraint that applies to all instances of a class.
