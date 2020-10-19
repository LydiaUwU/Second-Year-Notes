# Activity and Sequence Diagrams

## Activity Diagrams
Represents the workflow of a process and how activities are coordinated. They are particularly useful when you know that a process has to achieve a number of different things, and you want to model what the essential dependencies between them are, before you decide what order to do them.

Execution of steps can be both concurrent and sequential

## Three Features of Activity Diagrams
1. A transition may branch into two or more mutually exclusive transitions. **Guard expressions** label the transitions coming out of a branch. Denoted as *hollow diamonds*.
2. A transition may **fork** into two or more parallel activities. Denoted as *solid bars*.
3. Activity diagrams can be divided into object **swimlanes** that determine which object is responsible for which activity.

## Fork and Join
A for may have one incoming transitions and two or more outgoing transitions.

A join may have two or more incoming transitions and one outgoing transitions.

## Sequence Diagrams
**Sequence Diagram* Is an interaction diagram that details how operations are carried out.

Sequence diagrams are organised according to time.

The objects/actors involved in the operation are listed from left to right according to when they take part in the message sequence.

## Features of a Sequence Diagram
1. Each vertical dotted line is a **lifeline**, representing the time that an object exists.
2. Each **arrow** is a message call.
3. The **activation** bar represents the duration of execution of the message.
4. The expression in square brackets is a **condition**.
5. The diagram has a clarifying note, which is text inside a dog-eared rectangle.
