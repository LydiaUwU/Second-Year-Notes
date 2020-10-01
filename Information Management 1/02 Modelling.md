# Modelling

Models are *abstractions of the real world.

> There is no such thing as a "correct" model; models are simply better or worse suited to accomplishing a particular task

If systems are to be modeled care must be taken to consider all components. The behaviour of the systems is not the same as the sum of the behaviour of the system as a whole.

Modelling is required to *appropriately* automate systems.

## Why Use a Model?
A model is quicker and easier to build than the real thing and can be used in a simulation and can evolve as we learn. We can also choose what details to include in a model.
A model can represent real or imaginary things from any domain, using any materials.

# How Engineering Models are Used
1. To help us *understand* complex systems.
  - Useful for both *requirements* and *designs*.
  - Minimise risk by detecting errors and omissions early in the design cycle.
  - **To communicate understanding**.
2. To *drive implementation*
  - The model is a blueprint for construction.
3. To *reduce risk*.
4. To provide *different perspectives*.
  - We don't see everything at once.
  - We can use an easier to understand notation.

We need to be careful of scope creep when using a model.

## Why Use Diagrams in Modelling?
Convey meaning to others in an easy to understand and standardised way.

## Information Model
**Information Model:** A representation of concepts, relationships, constraints, rules and operations to specify data semantics for a chosen domain of discourse. Provides a complete set of views on the information for use by different stakeholders.

Typically technology neutral.

## Information Model Perspectives Views
Typical views are:
- **Structural/Static View:** How data and information is associated.
- **Dynamic Behaviour View:** What the user wants to do with the system, how the data interacts with each other.

## Origins of UML
Object-oriented analysis and design techniques.
UML's goal is to bring together the best features of all notations to produce an industry standard.
Applicable to any domain.

## What is UML and What is it Not?
UML is a specification and design language.
- Mostly visual but has semantics.
- Diagrams consist of well-defined elements and have rules on how to use and combine elements.
- Abstract syntax, well-formedness rules.

UML *is not a software tool*.
UML *is not a programming language*.

## What we are Going to learn

> You can model about 80% of problems using 20% of UML

### Use Case Diagrams
- Describe the functional behaviour of the system as seen by the user.

### Class Diagrams
- Describe the static structure of the system.

### Sequence and Activity Diagrams
- Describe the dynamic behaviour between objects of the system.
