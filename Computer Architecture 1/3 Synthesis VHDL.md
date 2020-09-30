# Synthesis and VHDL

VHDL describes the internal behaviour in the architecture construct.

- Synthesis produces a digital circuit that implements the behaviour captured in the VHDL description.
- VHDL is also the bases for a simulation.
- Characteristics of digital systems:
  - Structural.
  - Behavioural.
  - Physical.

Signals can be manipulated by gates as they are moved between registers. This process is clock dependent to keep everything in sync.

## Event, Propagation Delays and Concurrency
**Event:** When an input signal changes.
**Propagation Delays:** A delay between events. The time it takes for electrons to physically move through a circuit.
**Concurrency:** When multiple events occur at a time.

The clock speed has to take the propagation delay into account.

## Signals
- May be `0`, `1` or `Z`.
- Equivalent to wires in digital circuits.
- May be assigned values.
- Signals are associated with time values.
- Sequences of vales determines the waveform.

## Shared Signals
Hardware description languages must be expressive enough to describe signal that may be driven by one or more sources. This is sometimes called a 'Bus'.

## Design Entities
Design entities could be:
- Board
- Chip
- Gate
- Transistor

This design component behaviour must be described and simulated.

Design entities have the following:
- Input signals.
- Output signals.
- Behaviour. *E.g. Truth table, boolean equation, wires between gates, etc.*
- Two components in the design-entity description:
  - The Interface.
  - Internal Behaviours.

## Entity Declaration
Interface to design entitis through.

```VHDL
entity module is
  Port(x : in bit; y : out bit;)
end module;
```

**Ports:** Define the input and output of the design entitiy. Ports are signals that enable communication between the design entity and other entities.

Port signals must declare their type.
